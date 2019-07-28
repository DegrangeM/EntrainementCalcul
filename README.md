# EntrainementCalcul

Cet ensemble de fichiers LaTeX permet de générer des feuilles d'exercices aléatoires différent pour chaque élève.
Une correction contenant le résultat final est également fournis.

![image](https://user-images.githubusercontent.com/53106394/62010932-b6ee4480-b171-11e9-9d1f-32be138c6921.png)

Le fichier `main.tex` est le fichier à compiler. Vous pouvez y modifier :
- Le numéro de sujet (voir après) en modifiant la valeur 2 dans
```latex
%%%%%%%% DEFINITION DU NUMERO DE SUJET %%%%%%%%
%                                             %
                \def\Sujet{2}                 %
%                                             %
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
```
- Le nombre d'élèves en modifiant la valeur 10 dans
```latex
\foreach \n in{1,...,10}  {
```

Le fichier `exo.tex` contient la banque d'exercices disponibles

Le fichier `1.tex` contient les exercices du sujet n°1 ainsi que leur correction.

Même chose pour le fichier `2.tex`.

Lorsque le numéro de sujet est fixé à 2 dans `main.tex`, le pdf compilé va afficher les exercices du sujet n°2 ainsi que la correction du sujet précédent à savoir le sujet n°1.

Le fichier `0.tex` est un sujet vide qui permet uniquement au logiciel de continuer à fonctionner lorsque le numéro de sujet est fixé à 1 puisque celui-ci va alors tenter de charger la correction du sujet n°0.
