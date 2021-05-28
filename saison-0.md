
## Bienvenu à la saison 0. C'est ici que tout commence.

****

# <center> <b> <span style="color:orange;"> Programmation en Python </span> </b></center>

### <center> <b> <span style="color:green;">Des applications en Calcul Scientifique -  Statistiques -  Science des Données</span> </b></center>


****

# <center> <b> <span style="color:blue;">Variables et affectations</span> </b></center>



<!--NAVIGATION-->
<  [0. Introduction](00.Introduction_a_python.ipynb)| [Sommaire](Index.ipynb) | [2. Chaînes de caractères](02-Chaînes_de_caractères.ipynb) >



****



### <left> <b> <span style="color:brown;">Instructeur : </span> </b></left>[Yaé Ulrich Gaba](https://github.com/gabayae)




>    **Résumé:** Dès que l’on possède des *types de données*, on a besoin des *variables* pour stocker les
    données.
    En réalité, Python n’offre pas la notion de variable, mais plutôt celle de *référence d’objet*. Tant
    que l’objet n’est pas modifiable (comme les entiers, les flottants, etc.), il n’y a pas de différence
    notable. Dans le présent calepin, nous discutons les grandes lignes atour de l'utilisation des variables sous Python.
****

### Définir une variable

Sous Python, une variable est un objet de programmation permettant de stocker une
information en mémoire de la machine en attribuant un nom symbolique. Une variable est
définie en utilisant l’opérateur mathématique `=` soit par assignation directe de sa valeur, ou par
une assignation à partir de la valeur d’une autre variable. Exemples :


```python
x = 86 # définit la variable nommée x et lui assigne la valeur 86
```


```python
y = 4.8134 # définit la variable nommée y et lui assigne la valeur 4.8134
salutation = "Comment allez-vous ?" # Définit la variable nommée salutation et lui assigne la valeur " Comment allez-vous ?"
```

Pour afficher les valeurs des trois variables définies, on utilise la fonction **print()**-sur laquelle nous reviendrons quand nous parlerons des *objets fonctions sous Python*.


```python
print(x)
print(y)
print(salutation)
```

Pour afficher les trois valeurs sur la même ligne on utilise une seule fonction print() en séparant
les variables par des virgules :


```python
print(x,y,salutation)
```

Les examples présentes entrent dans le cadre de ce qe nous appelons `assignation directe`. Une `assignation multiple` est un cas d'`assignation directe` qui consiste à attribuer une même valeur à plusieurs variables dans la
même ligne de code. Exemple :


```python
x = y = 7 # x et y prennent la même valeur simultanément 7.
```

Une `assignation parallèle` consiste à définir plusieurs variables en utilisant un seul symbole
d’égalité. Exemple :


```python
x, y = 4, 8.33 # On définit deux variables x et y dont les valeurs sont respectivement 4 et 8.33.
```

<left> <b> <span style="color:red;">Affecter n’est pas comparer !</span> </b></left>
Il faut bien prendre garde au fait que l’instruction d’affectation `« = »` n’a pas la même signification que le symbole d’égalité `« = »` en mathématiques. Par exemple, le premier n’est pas
symétrique, alors que le second l’est : vouloir échanger l’ordre des éléments dans une instruction d’affectation produira immanquablement une erreur dans l’interpréteur :


```python
# Erreur
128 = a
```


```python
Ceci nous appelle a parler brièvement des noms de variables admissibles sous Python. 
```

####  <left> <b> <span style="color:brown;">Conventions de nommage </span> </b></left>

Les conventions de nommage des différents éléments de code sont importantes car elles donnent des informations supplé-
mentaires aux développeurs quant à la nature de certains attributs ou certaines variables.
La convention pour les noms de variable est la suivante:

   - Les mots réservés tels que `if`, `else` , etc., ne peuvent être utilisés comme noms de variables;
   - Les noms de variables peuvent debuter avec `_` , `$` , ou une lettre;
   - Les noms de variables peuvent etre en miniscule ou en majuscule;
   - Les noms de variables ne peuvent debuter avec un chiffre;
   - Les espaces blancs ne sont pas autorisés dans les noms de variables.

<left> <b> <span style="color:brown;"> Le bon programmeur s’efforce bien entendu de choisir les noms de variables les plus pertinents possible. </span> </b></left>

Sous Python, il existe **33** mots réservés dont la liste est fournie ci-dessous:

<center>
    <img src="images/python-keywords.png" width="50%">
    </center>

|             |                  |                  |                  |                  | 
|-------------|------------------|------------------|------------------|------------------|
|``and``      | ``elif``         | ``if``           | ``or``           | ``yield``        |
|``as``       | ``else``         | ``import``       | ``pass``         |                  | 
|``assert``   | ``except``       | ``in``           | ``raise``        |                  |  
|``break``    | ``False``        | ``is``           | ``return``       |                  |
|``class``    | ``finally``      | ``lambda``       | ``True``         |                  |
|``continue`` | ``for``          | ``None``         | ``try``          |                  |
|``def``      | ``from``         | ``nonlocal``     | ``while``        |                  |
|``del``      | ``global``       | ``not``          | ``with``         |                  |

**Remarque**: Python est sensible à la casse, ainsi, les noms de variables `Age` et `age` sont distincts. Suivant le langage, il y a une [convention de nommage](https://en.wikipedia.org/wiki/Naming_convention_(programming)#Python_and_Ruby) pour les variables qui est recommandée. 

- `UpperCamelCase` pour les noms de classe;

- `CAPITALIZED_WITH_UNDERSCORES` pour les constantes;

- `lowercase_separated_by_underscores` ou `snake_case` pour les autres variables.



[Revenir à la de garde](./)
