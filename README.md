# Dojo : Angular - ExportAs - ViewChild - Output 

Le but de ce dojo est de générer une phrase à partir d'un sujet (`SujetComponent`), d'un verbe (`VerbeComponent`) et d'un complement (`ComplementComponent`), via des techniques différentes.

L'application est composée de 5 components :
- `AppComponent` : composant root (contient uniquement `DashboardComponent`)
- `SujetComponent` : affiche une liste de prénom sélectionnable,
- `VerbeComponent` : affiche une liste de verbe sélectionnable
- `ComplementComponent` : affiche une liste de COD sélectionnable
- `DashboardComponent` : affiche les 3 composants (`SujetComponent`,`VerbeComponent` et `ComplementComponent`)

Il y a 3 techniques différentes pour arriver au resultat attendu. Voici les 3 mots clefs/concepts qui te permetteront de realiser ce dojo (classé du plus facile au plus difficile) :

1. ExportAs
2. ViewChild
3. Output

**Tu n'est pas obligé d'utiliser le bouton "Generer une phrase !!"**

## Gros bonus de ninja
Avec ton oeil aguerri de Wilder tu as surrement remarqué que les composants `SujetComponent`,`VerbeComponent` et `ComplementComponent` sont très similaires : même template HTML, même fonction `setSelected`, etc.\
Refactorise ton code pour ne plus avoir à utiliser `SujetComponent`,`VerbeComponent` et `ComplementComponent` mais à la place un component `ListWordsComponent` qui sera répété trois fois dans `DashboardComponent`.\
Il devra evidement prendre en entrée une liste de sujet ou de verbe ou de complement...`@Input()` et `<ng-content>` sont tes meilleurs amis pour ce bonus !!!
