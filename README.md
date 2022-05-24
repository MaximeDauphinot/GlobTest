# GlobTest

## Enoncé

[Echo](https://www.instagram.com/globalisecho/?hl=fr), mascotte de l'équipe de [Globalis](https://www.globalis-ms.com/), a découvert une fonction `foo()` bien mystérieuse. Hélas, il n'a pas accès au code. Curieux et grand amateur de [rétro-ingénierie](https://fr.wikipedia.org/wiki/R%C3%A9tro-ing%C3%A9nierie), Echo s'est amusé à appeler cette fonction, en injectant des données en entrée et en récoltant les sorties. Le comportement de la fonction `foo()` est le suivant :

| Appel                                                                |        Sortie         |
| -------------------------------------------------------------------- | :-------------------: |
| `foo([[0, 3], [6, 10]])`                                             |  `[[0, 3], [6, 10]]`  |
| `foo([[0, 5], [3, 10]])`                                             |      `[[0, 10]]`      |
| `foo([[0, 5], [2, 4]])`                                              |      `[[0, 5]]`       |
| `foo([[7, 8], [3, 6], [2, 4]])`                                      |  `[[2, 6], [7, 8]]`   |
| `foo([[3, 6], [3, 4], [15, 20], [16, 17], [1, 4], [6, 10], [3, 6]])` | `[[1, 10], [15, 20]]` |

Le challenge, si vous l'acceptez, serait d'aider Echo à comprendre ce que fait cette fonction et à la recoder. Vous êtes partant ? ;)

### Question 1

Expliquez, en quelques lignes, ce que fait cette fonction.

### réponse

La principe de la fonction est une sorte d'intersection entre des intervalles par exemple si l'intervale est inclu dans un autre intervale on le supprime pour éviter
les redondances.
La fonction prend en paramètre un tableau non trié, donc la première étape consiste à trier le tableau, ensuite, on vérifie deux par deux, si on trouver
une intersection entre les deux élements alors on fusionne les deux sinon on passe au suivant.
La fonction display permet juste d'afficher les résultats sous un format joli :)

### Question 2

Codez cette fonction.
Merci de fournir un fichier contenant :

- la fonction,
- l'appel de la fonction, avec un jeu de test en entrée,
- l'affichage du résultat en sortie.

### réponse

voir indedx.js

### Question 3

Précisez en combien de temps vous avez implémenté cette fonction.

### réponse

environ 5 min, la réponse étant dans les fork il m'a juste fallu lire quelques exemple pour comprendre et retranscrir la reponse qui me paraissait le plus adapté :)

## Merci

Par avance, un grand merci pour le temps que vous consacrerez à ce challenge, en espérant vous voir rejoindre très prochainement [nos équipes](https://www.globalis-ms.com/jobs/) ;)
