# Modèle proie/prédateur


### Membres du groupe :

 + BEAUREPAIRE Louis
 + DELATTE Thomas
 + GHAZI Virgile
 + PRAT Adélie
 
 
### Questions importantes autour du sujet :

 + Peut-on atteindre un état de stabilité entre les quantités de proies et de prédateurs ?
 + Peut-on modéliser efficacement les interactions entre les proies et les prédateurs et obtenir un modèle ressemblant à la réalité ?
  
  
### Phénomène principal étudié : interaction entre proies et prédateurs / évolution de leurs populations respectives.

⋅⋅⋅ Paramètres principaux entrant en jeu :

 + durée de vie des proies
 + durée de vie des prédateurs
 + taux de reproduction des proies
 + taux de reproduction des prédateurs
 + taux de consommation de nourriture des proies
 + taux de consommation des proies par les prédateurs
 + taux de renouvellement de la nourriture des proies

### Si ajout de spacialisation :
 + efficacité de recherche de nourriture des proies
 + efficacité de recherche de nourriture des prédateurs
 
 
### Méthodes de validation :

 + modèle proie/prédateurs pré-existants par comparaison
 + données de reproduction des lapins en Australie
 + vérification par comparaison avec le modèle Volterra/Lotka
 + études produites sur des éco-systèmes existants ?
 
 
### Premières idées de modélisation :
 + Idée n°1 : chaque agent a sa propre horloge interne et doit, à intervalles de temps réglés par nos paramètres, produire certaines interactions.
 
 ⋅⋅⋅ Cela permet d'avoir des comportements en apparence autonome obéissants aux mêmes lois. On empêche alors des effets de vague pouvant être causés par une mise en route aléatoire. Cependant l'initialisation des horloges internes doit être effectuée de manière à éviter des effets de vagues à répétition. De plus cela supprime toute potentialité de vagues, ce qui peut arriver dans la nature.

 + Idée n°2 : à chaque instant t toutes les interactions suivantes sont effectuées (le nombre de fois est dépendant des paramètres)
 
      * si une proie n'est pas nourrie, elle meurt
      * si une proie mange, une unité de nourriture disparait
      * chaque unité de nourriture produit potentiellement une autre unité de nourriture
      * si deux proies coexistent elles créent potentiellement une autre proie
      * si un prédateur rencontre une proie, la proie meurt
      * si un prédateur ne rencontre pas de proie, il meurt
      * si deux prédateurs coexistent elles créent potentiellement un autre prédateur

 + Idée n°3 : une spacialisation des agents
      
      ⋅⋅⋅ Cela permet d'avoir une représentation plus fidèle de la réalité par la suite, i.e. le rendu final sera probablement plus lisible et compréhensible. Cela implique cependant l'ajout de nouveaux paramètres.
 
 + Idée n°4 : Ø
 
 
### Taches et répartitions :

 + BEAUREPAIRE Louis : chef de projet - mise en code primaire
 + DELATTE Thomas : mise en code primaire - analyse secondaire
 + GHAZI Virgile : exploitation de l'idée - mise en code secondaire
 + PRAT Adélie : analyse primaire - mise en page
 


### Cahier de suivi : chacun inscrit les taches effectuées en suivant le modèle suivant

 + [NOM Prénom] - [JJ/MM] (si période [JJ/MM -> JJ/MM]) : [résumé en quelques mots]
 
        ⋅⋅* [Résumé plus approfondi]
        
 + Groupe - 27/02 : réunion de coordination
 
        ⋅⋅* Détermination des différents rôles
        ⋅⋅* Répartition des différentes tâches pour chacun dans la semaine à suivre
        
 + BEAUREPAIRE Louis - 27/02
 
        ⋅⋅* Mise en page et écriture du cahier des charges
