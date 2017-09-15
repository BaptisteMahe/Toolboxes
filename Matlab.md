# Matlab

___
## Variables

* ; à la fin d'une ligne ne renvoie pas de valeur
* les variables ne contiennent que lettres, nombres et _

___
## Mots clé

* ```clear ;``` : efface toutes les Variables
* ```clc```: clear the comand window
* ```save nomfichier nomvariable```: sauvegarde la variable nomvariable dans un fichier nomfichier.mat
* ```load nomfichier ```: charge la variable qui était enregistrée dans le fichier nomfichier.mat
* ```doc func```: ouvre la documentation de la fonction func
* ```plot(x,y,'color/line/marks')```: crée un graphique de y en fonction de x
___
## Fonctions / constantes

* pi
* i
* sqrt
* sin
* round : arrondi
* fft : crée la fft discrète d'une liste
* abs : valeur absolue

___
## Objets

###  arrays :

* Tout est scalaire
* LES INDICES COMMENCENT A 1
* ```a = [x y z]```
* ```a = first:spacing:last``` : crée un tableau ligne avec un espace par default de 1(```first:last```)
* ```a = linspace(first,last,number_of_elements)``` : crée un tableau ligne
* ne pas mettre d'espaces sur les côtés des sqared brackets
* séparation espace ou ```,``` : vecteurs ligne (row)
* séparation ```;```: vecteurs colonne (column)
* ```a = a'```transpose le tableau a
* rand(n) : crée une matrice de taille n*n contenant des nombres aléatoires entre 0 et 1
* rand(n,m) : crée une matrice de taille n*m contenant des nombres aléatoires entre 0 et 1
* zeros(n,m): crée une matrice de taille n*m contenant des 0
* array(n,m) : renvoie l'élément en place n,m du tableau arrays
  * n ou m peuvent etre ```end```, qui prend la derniere valeur possible
  * ```:```: prend en compte toutes les valeurs présentes dans cette dimension
* ```array(n,m) = valeur``` : mutateur
* ```max(array)```: renvoie la valeur maximale du tableau array
* ```[vmax,idmax] = max(array)```: place le max dans vmax, et son indice dans idmax
* multiplication:
  * ```*```: produit matriciel (attention à la compatibilité)
  * ```.*```: produit terme à terme
* ```dsize = size(data)``` : renvoie un vecteur contenant les tailles
* ```[dr,dc] = size(data)```: place les tailles des dimensions dans differentes variables
* ```numel(array)```:retourne le nombre d'elements dans array

### plots :


* ```hold on``` : permet de maintenir le graphe en place pour en placer un dessus
* ```hold off```: revient à la configuration initiale
* ```close all```: ferme tous les graphs
* ```plot(x,y,'color/line/marks')```: crée un graphique de y en fonction de x
* ```plot(x,y,'LineWidth', n)``` : la largeur du tracé est n
* example : ```plot(x,y,'ro-','LineWidth',5)```
* ajouter un titre : ```title('Plot Title')```
* label : ```ylabel(nomylabel)```: ajoute un label
* ajouter une legende  : ```legend('a','b','c')```

### booleans :

* 0 ou 1
* opérateurs :
  > < = & |
___
### fonction

* ```f = @(var) func(var)``` : f est la fonction qu iprend var en parametre et qui renvoie func(var)
* ```
  fonction res = nomfonction(var)
    res = actionsafaire(var)
  endfunction
```
