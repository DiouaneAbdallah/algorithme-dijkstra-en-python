# algorithme-dijkstra-en-python

Dans ce projet, nous allons traiter un problème d’optimisation, c’est la programmation des conducteurs d’un bus-navette d’un campus universitaire, de façon pour minimiser le coût total.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/dijkstraenpython.ipynb)

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

![Open In Colab](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image0.png)

### Le chemin le plus court :

Pour trouver le chemin le plus court nous allons utiliser la méthode de Dijkstra:

Itération 0 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image8.png)

Itération 1 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image7.png)

Itération 2 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image4.png)

Itération 3 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image2.png)

Itération 4 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image5.png)

Itération 5 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image1.png)

Itération 6 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image9.png)

Itération 7 :

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image3.png)

Le chemin optimal donné par cette méthode est :  19h -> 23h -> 02h

![algorithme-dijkstra](https://github.com/DiouaneAbdallah/algorithme-dijkstra-en-python/blob/main/images/image6.png)

