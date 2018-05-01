 # PRESENTATION DE LA THEMATIQUE 


Il s'agit ici de rendre compte de notions fondamentales sur lesquelles repose notre travail . 
On pourrait se pencher en premier lieu sur les **deux agents** que nous faisons intervenir, éléments clés autour 
desquels se construit notre programme . Il est donc nécessaire de définir brièvement ce terme . De ce fait, un
«agent» caractérise ce qui est à l'origine d'un processus ou d'un phénomène . 
Au sein de notre modélisation, les lapins et les renards endossent ce rôle : ils effectuent des déplacements et 
exécutent des actions selon leur état (si ils ont faim ou envie de se reproduire) . Ils déterminent donc les 
changements dans notre matrice espace de départ, en particulier la disparition de certains agents (lapins mangés ...)
et l'apparition de nouveaux (reproduction) . Un système d'**interaction** entre les agents est ainsi instauré, autre 
notion essentielle de notre travail . 

Une notion très importante intervient ici afin de lier les deux agents, c'est celle d'**interdépendance** . Dans notre cas,
c'est le rapport proie/ prédateur qui rend chacune des deux espèces dépendante de l'autre .
Cela rejoint bien tout l'enjeu de notre système à étudier l'équilibre d'un écosystème et voir si la cohabitation 
d'une population de proies et de prédateurs dans un milieu naturel est possible . 
Plus précisément, cette idée illustre le fait que le nombre de renards dépend de la quantité de ressources alimentaires 
disponible, soit le nombre de lapins . Réciproquement, la population de lapins diminue lorsque la population de prédateurs 
renards est élevée . Cette étude justifie l'ajout d'un agent «tiers», les carottes, qui représentent elle l'alimentation 
du lapin de laquelle dépend sa survie .  

Par ailleurs, il est nécessaire d'aborder la **simplification de la vie réelle** que constitue notre programme, notion capitale 
lorsqu'on réalise une modélisation . En effet, au cours de la création d'un projet visant à la simulation d'un phénomène 
existant, on fait le choix de l'intervention de certains facteurs et, à l'inverse, on en néglige d'autres . Par suite, le 
rendu n'est pas une représentation parfaite de ce qui se passe en pratique . Graphiquement, cela s'illustrerait par le fait 
que sur une courbe sinusoïdale, on ne prendrait en considération que la ligne médiane, approximation moyenne des processus 
rencontrés . 
Le choix des variables entrant en jeu est donc capitale pour espérer obtenir un résultat le plus proche possible de la réalité . En ce qui concerne notre travail nous avons donc tenté d'employer les caractéristiques qui nous semblaient cruciaux pour la 
mise en modèle de la réalité . A titre  d'exemple,             
nous pouvons mentionner en premier lieu la taille de la matrice qui pose le cadre de notre modélisation et le nombre de 
renards et de lapins (variable) que nous y faisons intervenir . La probabilité de présence de carottes intervient aussi, comme 
représentation de l’accès à la nourriture pour les lapins .On considère également l’espérance de vie, la maturité sexuelle ou 
encore le temps de gestation de chacune des deux espèces ainsi que l’efficacité/chance de réussite de la chasse du renard  
(sur la base de données réelles ) . Enfin, les seuils d’excitation et de faim de chaque animal -déterminant  la façon dont 
il va agir : manger ou se reproduire- et le gain d’excitation et de faim résultant de chacune de ces interactions sont pris 
en compte .
Bien que pourvu de nombreuses variables, cela s'apparente à une simplification de la vie réelle . En effet, ici on ne prend 
notamment pas en compte les aléas qui pourraient survenir dans la réalité tels que les maladies, les blessures entraînant 
la mort ainsi que les cas de fausse-couche, stérilité empêchant la reproduction, ou encore la présence d'autre animaux dans 
le régime alimentaire du renard .  
Là se situe donc tout l'intérêt de la vérification avec les données existantes et les travaux déjà menés . 
