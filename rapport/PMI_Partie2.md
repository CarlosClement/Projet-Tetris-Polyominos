# PROJET MATH INFO PARTIE 2

### Idées :

> **comment généraliser cela pour les dimensions supérieures**

> **Interfaces différentes (pas forcément des rectangles) / mods différents**

> **Creer un chemin d’un point a a un point b a l’aide de polyominos**



### PARTIE 2.1

#### 1
Nous avons decide de representer les polyominos sous formes de matrices en 2 dimensions.
Les 1 representent les cases prises par le polyominos et les cases 0 representent les cases vides.

 Par exemple:
```
[[0,1,0],[0,1,0],[1,1,1]] donne le polyomino:

  []
  []
[][][]  soit,   [[0,1,0],
                 [0,1,0],
                 [1,1,1]]
```

#### 2
Pour obtenir les classes de rotation et de symetrie d'un polyomino donne,
il suffira de de tourner notre matrice 3 fois a 90 degres car la 4ème fois reviens a la matrice initiale.
Puis on fait de meme en commencant par une matrice inverse.


#### 3
Pour tester que 2 polyominos appartiennent a la meme classe complete,
il suffit de faire la rotation de l'un jusqu'a obtenir l'autre 
et si la rotation ne fonctionne pas on inverse le premier et on refait une rotation.
Apres ces 2 rotations, si l'on na pas obtenu le second polyomino alors c'est qu'ils n'appartiennent pas a la meme classe complete.


#### 4
PERPLEXE: Pour representer le pavage d'une zone donnee, il nous faut la liste de polyominos avec lesquelles on va paver la zone. on essayera ensuite demboiter les polyominos entre eux jusqu'a ce que la zone donnee qui sera representee par un matrice soit remplie de 1. Si elle ne peut etre remplie par les polyominos alors on envoie un message d'erreur. La zone ne sera pas obligatoirement carree, on representera les zones mortes par de croix. Par exemple:

```
[[x,x,x,0,0],
 [0,0,0,0,0], sera la zone a paver et [1] et [1,1] seront nos polyominos
 [0,0,0,0,x],
 [0,0,0,0,0],
 [x,x,0,0,0]]
 
 On remarque donc qu'il y a plusieurs pavages possibles --> A ETUDIER ! 

```


### PARTIE 2.2



### PARTIE 2.3


### PARTIE 2.4


