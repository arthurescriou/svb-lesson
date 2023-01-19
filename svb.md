# Communication

On veut faire communiquer nos vaisseaux. Pour ça on a besoin de format de message stable et typé.

## Propager le radar

On envoi seulement les positions ennemi par messages.

Point positif:

- on peut les utiliser comme notre propre radar dans le code (il faut vérifier la portée avant)

Point négatif:

- il peut y avoir des redondances
- il y a un risque que plusieurs vaisseaux tire sur la même cible (pas de coordination)

## Donner des ordres

On veut maintenant centraliser la décision: un seul vaisseaux donne des ordres et les autres execute.

On peut imaginer plusieurs type d'ordres:

- attaquer: tirer sur une cible (ou suivre un ennemi si pas à portée)
- patrouiller: se déplacer vers une position et attendre à cet endroit
- reconnaissance: avancer tout droit pour trouver les ennemis
- protéger un autre vaisseaux: suivre le déplacement d'un autre vaisseaux

Chacun des vaisseaux doit toujours partager ses informations radar et sa position.

Au début de la partie les vaisseaux de l'équipe doivent s'identifier auprès du leader: envoyer un message avec leur identifiant et leur statistique.
