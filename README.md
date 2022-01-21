# algorithme-dijkstra-en-python

Dans ce projet, nous allons traiter un problème d’optimisation, c’est la programmation des conducteurs d’un bus-navette d’un campus universitaire, de façon pour minimiser le coût total.

Premièrement, nous allons modéliser le problème, par un graph, ensuite en utilisant la méthode de Dijkstra nous allons essayer de trouver la programmation optimale.

### Présentation du problème :

L’objectif est de minimiser le cout d’un bus-navette en respectant les contraintes suivantes :
- Le bus commence de 19h à 2h.
- Plusieurs conducteurs assurent le service.
- seulement un conducteur doit assurer le service à tout moment.
- Si elle commence à 21h ou avant, un conducteur régulier peut être engagé pour 4h de service qui coûtera 50 $.
- Si non, plusieurs conducteurs à temps partiels peuvent assurés le service de 3h qui coûtera 40$, et le reste est limité à 2h de travail qui coûtera 30$.

### Modélisation du problème :

Nous allons modéliser ce problème sous forme d’un graphe, en considérant les heures de 19h
à 2h, comme les sommets du graphe, et les couts des conducteurs comme des valeurs des
arcs.
Nous avons obtenu le graphe suivant :



### Le chemin le plus court :

Pour trouver le chemin le plus court nous allons utiliser la méthode de Dijkstra:

Itération 0 :


Itération 1 :


Itération 2 :


Itération 3 :


Itération 4 :


Itération 5 :


Itération 6 :


Itération 7 :


Le chemin optimal donné par cette méthode est :  19h -> 23h -> 02h
