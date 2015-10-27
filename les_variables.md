# Les variables

Une variable est un objet repéré par son nom. Elle peut contenir tout type de donnée et être modifiée lors de l'exécution du programme.

En JavaSript le nom d'une variable doit répondre à certains critères :

1. il doit commencer par une lettre (majuscule ou minuscule) ou un `_` underscore.
2. il peut comporter des lettres, des chiffres et les caractères `_`et `&`.
3. **les espaces ne sont pas autorisés**
4. Les noms de variables ne peuvent pas être les noms réservés suivants :<br/><small>*abstract, boolean, break, byte, case, catch, char, class, const, continue, debugger, default, delete, do, double, else, export, extends, false, final, finally, float, for, function, goto, if, implements, import, in, infinity, instanceof, int, interface, label, long, native, new, null, package, private, protected, public, return, short, static, super, switch, synchronized, this, throw, throws, transient, true, try, typeof, var, void, volatile, while, with.*</small>

## Création de notre première variable

Nous déclarons notre variable.
```js
var maVariable;
```

Le mot clé **var** indique que vous déclarez une variable. Le point-virgule `;` indique que l'instruction est terminée.
Une fois déclarée, **var** n'est plus nécessaire, vous pouvez stoker ce que vous souhaitez.

```js
var maVariable;
maVariable = "J'aime JavaScript";
```

Nous pouvons modifier sa valeur.

```js
var maVariable;
maVariable = "J'aime JavaScript";
maVariable = "Je n'ai pas peur de JavaScript";
// maVariable vaut "Je n'ai pas peur de JavaScript
```

Nous pouvons déclarer une variable et lui attribuer une valeur sur la même ligne.

```js
var maVariable_2 = 7;
```

Nous pouvons déclarer plusieurs variables sur une ligne, mais attribuer une valeur seulement à *maVariable_*2.

Lorsque l'on déclare des éléments de même type, il n'est pas nécessaire de répéter le mot clé `var`. Il suffit de séparer chaque déclarations par une virgules.

```js
var maVariable_1,
    maVariable_2 = 7,
    maVariable_3;
```

Avec le code ci-dessous, vous afficherez la valeur de votre première variable dans la console d'un navigateur.

```js
var maVariable = "J'aime JavaScript";
console.log(maVariable);
```
