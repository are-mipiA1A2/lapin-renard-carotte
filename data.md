## Informations sur le lapin utile au coodage

### Durée de vie :
- 9 ans 
- 30% de morts tous les ans  

### Relatif à la fécondité :
- maturité sexuelle : dès 9-12 mois 
- gestation 29 à 35 jours 
- période d'accouplements de 4 à 6 jours tous les 10 jours 
- 4 à 12 lapereaux par portée 

### Espace géographique : 
- groupes familiaux 1-5 mâles, 1-6 femelles 
- s'éloigne jusqu'à 150-400 m de leur terrier 
- surface occupée : 9 à 10 hectares
- vitesse de déplacement : 30 à 40 km/h 

## Données sur le renard utile au codage

### Durée de vie :
- 7 à 9 ans (souvent beaucoup moins)
- 80 % ne survivent pas à la première annnée

### Relatif à la fécondité :
- maturité sexuelle : 10 mois 
- gestation de 49 à 58 jours 
- accouplement 1 fois/an, 3 jour de fécondation possible au maximum
- 4 à 5 renardeaux/ portée 

### Besoin en nourriture : 
 - 500 g/jour 

### Espace géographique : 
- territoire de chasses : 150 à 350 hectares 
- vitesse de déplacement : 6 à 13 km/h (sprint : 60 km/h)

### Ebauche de fonctions :
- fonction interaction lapin-renard : 

    On évalue la probabilité pour le renard d'attrapper sa proie à 1/5 à laquelle on ajoute une valeur d'habileté du renard 
    variant de -1/10 à +1/10 . On notera cette habileté mu 
 
    On évalue la capacité du lapin à s'échapper à 0 plus ou moins 1/10 (noté epsilon)

    Probabilité de réussite de la chasse : **1/5+mu-epsilon** 
    
 - nombre de renardeaux par case à l'issu d'une interaction renard-renard : si moyenne fécondité deux renards < 0.5 alors 
   pas de portée sinon nombre aléatoire de petits renards entre 4 et 5 
   
 - 
