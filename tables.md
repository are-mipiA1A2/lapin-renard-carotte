 ## Tableau Attribut de l'agent renard


| Nom       | Type          | Intervalle  |Valeur Initiale | Fixe |
| ------------- |:-------------:| -----:|:-----:|:-------:|
| Sexe      | Bool | / | True ou False   | oui |
| Efficacité      | Float      | [1/10 ; 3/10] | entre 1/10 et 3/10  |oui  |
| Age | Int      |    [0 ; 1825] | 0 |non   |
|Fécondité | Float | [0 ; 1] | entre 0 et 1 |oui |
|Faim | Float | [0 ; 1] | 0 | non |
| Excitation | Float | [0 ; 1] | 0 | oui |
| Position | Tuple de (x:int,y:int) | / | / | oui |
| Gestation | tuple de bool et de deux int | / |(False, 0, 0)| oui |

 ## Tableau Attribut de l'agent lapin 
 
 
 
| Nom       | Type          | Intervalle  |Valeur Initiale | Fixe |
| ------------- |:-------------:| -----:|:-----:|:-------:|
| Sexe      | Bool | / | True ou False   | oui |
| Efficacité      | Float      | [-1/10 ; 1/10] | entre 1/10 et 3/10  |oui  |
| Age | Int      |    [0 ; 2000] | 0 |non   |
|Fécondité | Float | [0 ; 1] | entre 0 et 1 |oui |
|Faim | Float | [0 ; 1] | 0 | non |
| Excitation | Float | [0 ; 1] | 0 | oui |
| Position | Tuple de (x:int,y:int) | / | / | oui |
| Gestation | tuple de bool et de deux int | / |(False, 0, 0)| oui |


## Tableau Attribut de l' "agent" carotte 

 
| Nom       | Type          | Intervalle  |Valeur Initiale | Fixe |
| ------------- |:-------------:| -----:|:-----:|:-------:|
| Position      |Tuple de (x:int,y:int)| / | / |oui |
| Densité       | Float      | [0 ; +∞ ] | | oui |

 
 ## Tableaux des Paramètres 
 
 
| Nom       | Type          | Intervalle  |Valeur Initiale | Fixe |
| ------------- |:-------------:| -----:|:-----:|:-------:|
| Taille matrice | Int | / | 100 | oui |
| Range | Int| [0 ; 4] | ∅  |oui  |
|Gain de densité des carottes | Float      |    [0 ; 1] | / |non   |
|Espérance de vie lapins | Int | ∅ | 2555 |oui |
|Espérance de vie renards  | Int |∅| 1825 | oui |
| Maturité sexuelle lapins | Int | ∅ | 124 | oui |
| Maturité sexuelle renards | Int | ∅ | 310 | oui |
| Temps de gestation renard/lapin | Int | ∅ |55| oui |
| Seuil faim renard | Float | [0 ; 1] | 0 | non|
| Seuil excitation renard  | Float| [0 ; 1] | 0 |non |
|Seul faim lapin | Float      |    [0 ; 1] | 0 |non |
|Seuil excitation lapin | Float | [0 ; 1] | 0 |non |
|Espérance de vie renards  | Int |∅| 1825 | oui |
| Nombre de renard | Int | [0 ; 1000] | / | non |
| Nombre de lapins | Int | [0 ; 2000] | / | non |
| Probabilité de présence de carotte | Float | [0 ; 1] |/| non |
| Gain d'excitation renard/lapin | Float | [0 ; 1] | / | non |
| Gain de faim | Float | [0 ; 1] |/| non |

## Tableau Indicateurs 

| Nom       | Type          | Intervalle/Ensemble de valeurs |
| ------------- |:-------------:| -----:|
| Population Renard | Int |[0 ; 1000] |
| Population Lapin | Int| [0 ; 2000] |
| Densité Carotte | Float | [0 ; 1] |


|Liste des Expériences |
| ------------- |
| Faire varier Nombre de Lapin |
| Faire varier Nombre de Renard |
| ??Faire varier seuil d'excitation/faim?? |
| Faire varier gain d'excitation/faim |
| Faire varier gain de densité des carottes/ probabilité de présence|



 
 

 
 
