# Que sont les variables ?  

**Les variables** permettent de stocker des données dans notre programme. Elles sont placées dans la mémoire vive et doivent être **déclarées** (crées) avant de pouvoir être utilisées.

Pour cela, elles ont besoin de plusieurs caractéristiques :
  * un **nom** : un nom sous lequel elle sera accessible dans notre code.
  * un **type** : il définit ce que la variable peut contenir (maximum, minimum, sa taille etc...). Le système d'exploitation alloue une partie de la mémoire vive différente en fonction des types utilisés donc veillez à **bien choisir le type** de variable.
  * une **valeur** : c'est le contenu de la variable, elle peut varier en fonction du temps si elle n'est pas déclarée [constantes](#constantes).
  * une **portée** : c'est la portion de code (la zone de code) où elle est utilisable.
  * une **visibilité** : ce sont les règles qui fixent qui a accès à cette variable (qui peut la voir et l'utiliser. ex: uniquement la méthode, la classe, le package, tout le projet...).
  * une **adresse** : ou l'endroit de la mémoire où elle est stockée.
    > Ne concerne pas Java \(voir [les références](references.md)\) dans la suite.

  * une **durée de vie** : si la variable n'est utilisée qu'une fois, elle n'a pas besoin d'exister pendant toute la durée du programme.

> **[danger] Attention**
>
> La **portée** et la **visibilité** sont deux choses bien **distinctes** malgré qu'elles soient liées. Beaucoup de personnes ne perçoivent pas la nuance mais elle est bien présente.

Si on définit une variable ainsi :  

![](assets/var-def.png)  

Imaginons un programme ainsi :  

![](assets/program.png)  

> **[info] Info**
>
> Ici, **int** est le **type de variable**. Il s'agit d'un **nombre entier**.  

### Description  

Notre programme est composé de **3 parties** :
  * Calcul de la moyenne
  * Calcul de la somme
  * Calcul du produit des deux

Les variables de la **moyenne** ont une portée et une visibilité qui est la zone bleue. Les variables de la **somme** ont une portée et une visibilité qui est la zone violette. ElleS sont ni visibles, ni accessibles de l'extérieur.   
Les portées sont dites de la méthode car les variables peuvent être détruites une fois le calcul effectué.  
Mais, nous avons deux exceptions ! _**résultat**_ peut voit les valeurs _**moyenne**_ et _**somme**_. On a changé leurs visibilités pour qu'elles soient accessibles dans le reste du programme.  

## Déclarations
{% method -%}
On déclare une variable ainsi :
{% sample lang="java" -%}
```
<Type de la variable> <Nom de la variable> = <Valeur de la variable>;
```
ce qui donne dans le code :
{% sample lang="java" -%}
```java
int entier = 42; // Notre variable de type int contient la valeur 42.
// Plus tard...
entier = 24; // On change la valeur de notre variable
```  
{% endmethod %}  

Le point-virgule signifie **la fin d'une instruction**. Nous les reverrons plus tard.

> **[danger] Attention**
>
> Une variable du type **XYZ** ne peut contenir que des données du type **XYZ**.

## Constantes  

{% method -%}
Les **constantes**, comme indique leur nom, sont des variables dont la valeur **ne change jamais** une fois déclarée. Elles s'écrivent avec le mot-clé ``final``.

{% sample lang="java" -%}
```java
final int entier = 42; // Notre constante de type int contient la valeur 42.
entier = 24; // Erreur
```  
{% endmethod %}  
