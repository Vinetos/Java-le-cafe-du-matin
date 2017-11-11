# References  

Si vous avez des connaissances dans d'autres langages tels que le C++, ce terme de **références** ne vous est pas inconnu.  
Une référence peut être vue comme un **alias d'une variable**. C'est-à-dire qu'utiliser la variable, ou une référence à cette variable est équivalent. Ce qui signifie que l'on peut modifier le contenu de la variable en utilisant une référence.  
Vous allez voir que ce comportement de Java est particulier par rapport aux autres langages.

## En c++
{% method -%}
En C++ par exemple les références se manipulent ainsi :  
{% sample lang="java" -%}
```c++
int a = 0; // On crée une variable qui vaut 0
int& r = a; // On crée une référence de a qu'on appelle r
r = 12; // r = 12 équivaut à faire a = 12

// a vaut 12
```   
{% endmethod %}  
{% method -%}
Dans une méthode cela donnerait :

{% sample lang="java" -%}
```c++
void addOne(int& r) { // On crée en paramètre une référence de a qu'on appelle r
  r += 1; // On ajoute un à la référence et on ajoute un
}
// Plus tard...
int a = 0; // On crée une variable qui vaut 0
addOne(a); // On utilise la fonction avec en paramètre a

// a vaut 1
// r vaut 1
```   
{% endmethod %}  

On voit que le symbole ``&`` déclare que la variable sera une référence sur une autre variable de type ``int``.  

## Java
{% method -%}
Avec Java, c'est un petit peu plus complexe. Les références se sont pas explicites et ne sont possible que sur les **objets**.

{% sample lang="java" -%}
```java
int a = 0; // On crée une variable qui vaut 0
int r = a; // On copie la valeur de a et on la met dans une nouvelle variable qui s'appelle r
r = 12; // On change la valeur de r

// a vaut 0
// r vaut 12
```   
{% endmethod %}  

Lorsqu'on utilise des [variables primitives](primitives.md), Java copie la variable et ne crée pas de références.  

{% method -%}
Si on utilise un objet cela change :  
J'ai créé mon objet **Test** qui contient une variable **String** appelée **message**.

{% sample lang="java" -%}
```java
Test t1 = new Test();
t1.message = "Bonjour";

Test t2 = t1;
t2.message = "Salut";

// message de t1 vaut "Salut"
// message de t2 vaut "Salut"
```   
{% endmethod %}  

Comme on le voit, ``t2`` sert de référence à ``t1``. Donc si on modifie ``t2``, ça modifie ``t1``.

{% method -%}
Mais dans une méthode cela se passe différemment :

{% sample lang="java" -%}
```java
void changeMessage(Test t2) { // On demande un paramètre qu'on appelle r
  t2.message = "Salut"; // On ajoute un
}
// Plus tard...
Test t1 = new Test();
t1.message = "Bonjour";
changeMessage(t1);

// message de t1 vaut "Bonjour"
```   
{% endmethod %}  

Comme on le voit, on a créé une copie de la variable ``t1`` qui sera utilisée dans la fonction, que ça soit un objet ou non.  
