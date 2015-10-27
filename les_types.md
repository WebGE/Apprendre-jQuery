# Les types

## Les chaînes de caractères ou "string"

Ce type représente un texte quelconque.
On peut l'assigner de deux façons différentes.

**Avec des guillemets**
```js
maVariable = "J'aime JavaScript";
```

**Avec des apostrophes**

```js
maVariable = 'J\'aime JavaScript';
```

**Attention**, si vous utilisez des apostrophes dans la déclaration et que le texte en contient aussi, vous devez échapper les apostrophes contenus dans le texte avec le caractère `\` (antislash).
Dans le cas contraire, JavaScript pensera que le code s’arrête à la première apostrophe et produira une erreur.

## Le type numérique ou "number"

Ce type de variable représente tout les nombres (entiers et réels).

```js
maVariable = 3;
```

Le séparateur utilisé pour les nombres réels est le point et non la virgule.
```js
maVariable = 3.5;
```

**Attention**, si vous placez un nombre entre guillemets ou entre apostrophes, il sera reconnu comme une chaîne de caractères.
```js
maVariable = '3'; // Chaîne de caractères
```

## Les booléens

Un booléen désigne une variable ne pouvant prendre que deux valeurs **true** ou **false**.

Lorsque :

* aucune valeur n'est passée ;
* la valeur est égale à *0* ;
* une chaîne de caractères est vide, *null*, *undefined* ou *NaN*

la valeur de l'objet est initialisée à `False`.

Dans tous les autres cas, l'objet Boolean possédera la valeur `True`.

Une variable booléenne est assignée de la façon suivante :

```js
var isTrue = true;
var isFalse = false;
```

## Test de type

Le type d'une variable se vérifie avec l’instruction **typeof**.

La fonction **console.log()** affiche le résultat dans la [console](http://www.alsacreations.com/astuce/lire/1436-console-javascript.html) du navigateur.

```js
var myVariable = 2;
console.log(typeof myVariable); // Affiche : « number »

var myVariable = 'Mon texte';
console.log(typeof myVariable); // Affiche : « string »

var myVariable = false;
console.log(typeof myVariable); // Affiche : « boolean »
```

L’existence d'une variable se vérifie avec la même instruction.

```js
console.log(typeof otherVariable); // Affiche : « undefined »
```

## La convertion de type

### Convertion du type "string" en type "number"

Il peut être nécessaire de convertir une chaîne de caractères en un nombre. La méthode `parseInt()` effectue cette conversion.

```js
var myVariable = '2',
    n = parseInt(myVariable);
console.log(typeof n); // Affiche : « number »
```

### Convertion du type "number" en un type "string"

La méthode `toString()` convertie un nombre en une chaîne de charactères.

```js
var myVariable = 2,
    n = myVariable.toString();
console.log(typeof n); // Affiche : « string »
```

















