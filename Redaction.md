# Trace écrite 

Groupe composé de Louis Beaurepaire, Thomas Delatte, Virgile Ghazi et Adélie Prat 

## Présentation du projet 

Le projet sur lequel nous travaillons s'intitule "Equilibre d'un écosystème" . 

Il consiste en la modélisation interdépendante de deux populations : proies et prédateurs . 
Plus particulièrement, on s'intéresse ici à l'évolution du nombre de renards et de lapins au sein 
d'un même milieu, l'objectif étant de déterminer si un état d'équilibre du rapport proie/prédateur 
est possible et sous quelles conditions il est atteint . 

Afin de répondre au mieux à cette problématique, plusieurs questions seront soulevées telles que 
"Si un tel équilibre est possible alors pour quelles valeurs est-il obtenu ?" ou encore "Quelles sont 
les variables pertinentes à prendre en compte pour modéliser efficacememt les interactions proies/prédateurs ?" .
Enfin, à l'issu de sa réalisation, une dernière question constituera l'analyse critique de notre modèle :
"Dans quelles mesures celui-ci est-il ressemblant à la réalité et quelles en sont les limites ?" . 

## Déterminations des Paramètres de notre modèle 

Dans le cadre du phénomène que l'on étudie, plusieurs paramètres entrent en jeu : 
Nous pouvons mentionner en premier lieu la taille de la matrice qui pose le cadre de notre modélisation 
et le nombre de renards et de lapins (variable) que nous y faisons intervenir .
La probabilité de présence de carottes intervient aussi, comme représentation de l'accès à la nourriture
pour les lapins .
On considère également l'espérance de vie, la maturité sexuelle ou encore le temps de gestation de chacune 
des deux espècesainsi que l'efficacité/chance de réussite de la chasse du renard (sur la base de données 
réelles ) . 
Enfin, les seuils d'excitation et de faim résultant de chacune de ces interactions sont pris en compte .
Le choix de tels paramètres permettra à l'issue du projet la représentation de la population de chacune
des espèces renard, lapins et carottes au cours de temps . 

## Fonctionnement du Programme 

Notre modèle s'effectue de la manière suivante :

Premièrement nos agents sont spatialisés sur une matrice de taille n=100 .  
On définit les variables pour chaque agent au sein de cette environnement avant de déterminer les fonctions 
de déplacement .
Tout d'abord, on met à jour les paramètres de chaque agent, renard et lapin pour chaque jour : les seuils
de faim, d'excitation ainsi que l'âge augmente, l'animal disparaît si son espérance de vie est dépassée ou 
si la faim est trop forte (>1 dans notre programme) . De même, pour une femelle en gestation, si le compteur 
indique la fin de la durée de gestation alors des petits en nombre aléatoire sont crées et le compteur retombe 
à zéro .

On détermine ensuite les différentes interactions possibles :

▪	Si la faim du renard est supérieur au seuil de départ (celui pour lequel l’agent n’a ni faim ni envie de se 
 reproduire) et au seuil d’excitation et qu’il y a une carotte près de lui ou s’il il est davantage excité mais 
 qu’il n’y a pas d’autre renard à proximité  alors dans le cas où il parvient à attraper le lapin (paramètre efficacité
 de chasse ) celui-ci est mangé et disparaît de la matrice . Le renard prend alors la position de la proie qu’il a tué
 et son seuil de faim prend la valeur 0 .   


▪	En revanche, si l’excitation est supérieure au seuil de départ et qu’un renard se trouve à proximité ou si le renard
  a davantage faim mais qu’il n’y a pas de lapin aux alentours, alors dans le cas où le renard à proximité est du sexe opposé
  (avec un seuil d’excitation suffisamment élevé) et si le renard femelle n’est pas en gestation alors il y a reproduction 
  et un nombre aléatoire de renardeaux sera crée sur la position de la femelle lorsque le compteur de gestation arrivera à 
  son terme . Le renard de départ prend la position du renard avec lequel il s’est reproduit et le seuil d’excitation de 
  chacun des deux renards prend la valeur 0 . Dans le cas où il n’y a pas reproduction, le renard se déplace et occupe une 
  place aléatoire .  
  
  En ce qui concerne les lapins, les interactions se font de la même façon, seules les proies changent et deviennent les 
  carottes . On précise que la densité de carottes augmente au cours du temps  (?) . 
  
## Mode de Vérification 

Dans la dernière partie de notre projet nous seront chargés de valider notre modèle . Pour cela, nous nous appuierons sur 
différentes études ayant été menées auparavant mais aussi les écrits portant sur les conséquences de l'introduction du lapin
dans l'écosystème australien et notamment les données sur sa reproduction . En outre, on pourra ajouter un autre interêt à 
notre travail en se penchant sur un modèle bien connu de rapport proie/prédateur, celui de Volterra-Lotka (s’appuyant sur 
l’étude conduite par la Compagnie de la Baie de Hudson au 19e siècle sur une population de lynx et de lièvre), afin de  le 
comparer au notre (par le biais des graphiques obtenus par exemple) .

## Liens Utiles : 

- Conséquences introduction lapins écosystème australien (soulève l’incroyable capacité des lapins à se reproduire vite + gros impact sur végétaux et autres espèces)
https://www.futura-sciences.com/planete/dossiers/zoologie-especes-animales-invasives-1093/page/2/
http://www.liberation.fr/sciences/1996/01/16/hecatombe-de-lapins-australiens-plus-de-dix-millions-sont-deja-morts-histoire-d-une-bavure-scientifi_160045
http://www.linternaute.com/science/biologie/dossiers/06/0604-especes-invasives/lapin.shtml

- Volterra-Lotka : 
https://fr.wikipedia.org/wiki/Équations_de_prédation_de_Lotka-Volterra
http://www.tangentex.com/LotkaVolterra.htm
exposé déjà mené sur le sujet : https://www-fourier.ujf-grenoble.fr/~parisse/irem/proies_predateurs_diaporama.pdf

- Explication du comportement proie/prédateur (appui pour vérification) - p.5, 6 et 16 
https://www.aquaportail.com/definition-11184-relation-predateur-proie.html





