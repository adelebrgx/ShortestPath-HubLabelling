# Présentation

## Précalcul

0. Ecrémage :
    * O(N) pour exclure la région parisienne
    * O(1) pour sélectionner les n plus grandes villes dans une liste triée et ajouter Paris

1. Conception d'un réseau de routes factices :
    * O(n²) pour calculer toutes les distances et n'ajouter une route que si la distance est inférieure à une certaine distance max

2. Dijkstra sur toutes les villes reliées à Marseille :
    * O(n²) pour Dijkstra entre Marseille et une destination donnée
    * O(n^3) pour Dijkstra entre Marseille et chacune des n-1 autres villes

3. Dijkstra avec toutes les villes comme sources, pour toutes les destinations :
    * O(n^4) pour Dijkstra entre la ville V et chacune des n-1 autres villes, pour toutes les n villes.

4. Détermination des hubs pour chaque ville :
    * O(n^3) dans le cas le pire

Total précalcul : O(n^4), où n est la taille du subset de villes qu'on a sélectionné dans la carte de France pour des raisons de simplicité.

## Calcul temps réel

Une fois qu'on a tous les hubs en mémoire, il suffit de calculer quelques hubs par récurrence entre le départ et la destination. La complexité dépend du niveau de précision requis, mais elle est maîtrisée.
