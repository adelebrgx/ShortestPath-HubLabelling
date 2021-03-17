# ShortestPath-HubLabelling

## Plan de bataille

1. Ecrémer la liste des villes en ne conservant que les 50 les plus peuplées, en excluant la région parisienne sinon il y aura beaucoup de villes au même endroit
2. Relier toutes les villes entre elles via un réseau routier factice
3. Trouver les routes les plus courtes de Marseille à toutes les villes
4. Couper ces routes au 2/3.
5. Dans le 2ème tiers, sélectionner (déterministiquement) une ville qui sera le hub pour Marseille.
6. Ainsi, on a la liste des hubs de Marseille.
7. Recommencer pour toutes les autres villes.
