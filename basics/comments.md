# Les commentaires  

Les commentaires sont des lignes dans notre code qui vont être ignorées lors de la compilation et l'exécution du programme.  
Ils nous permettent d'expliquer des parties de codes compliquées. Ils sont utiles voire indispensables dès lors que l'on travaille en équipe, afin de faciliter la compréhension du code.

#### Les commentaires réguliers

Il existe deux types de commentaires dits « **réguliers** » :  
{% method -%}
**Sur une ligne** :  
{% sample lang="java" -%}
```
// Ce commentaire ne couvre qu'une ligne et ignore tout ce qui se trouve jusqu'au prochain retour à la ligne.
```  
{% endmethod %}
{% method -%}
**Sur plusieurs lignes** :  
{% sample lang="java" -%}
```
/* Ce commentaire couvre tout ce qui
   se trouve jusqu'ici */
```  
{% endmethod %}

> **[info] Note**
>
> **L'avantage** de ces commentaires est qu'ils peuvent être **utilisés** dans **n'importe quel contexte**.  

```java
public/* Ici */ static void main(String[] args) {/* Là */
    System./* ou encore ici */out.println("Hello World !");
}/*et pourquoi pas là ?*/
```

#### La javadoc  
{% method -%}
Un certain type de blocs de commentaires sont utilisés pour créer la **javadocs**. Pour faire simple, ils permettent de créer des sites web expliquant comment le code fonctionne. Nous reverrons cela plus tard.
En voici un exemple :  
{% sample lang="java" -%}
```java
/**
  * La méthode principale de mon programme.
  * Elle affiche <code>Hello World !</code> dans la console
  * @param   param1  un premier paramètre
  * @param   param2  un second paramètre
  */
public static void main(String[] args) {
    System.out.println("Hello World !");
}
```
{% endmethod %}  

# Utiliser les commentaires
{% method -%}
Les commentaires s'utilisent n'importe où dans le code.  
{% sample lang="java" -%}
```java
/**
  * Ce commentaire est appelé "header" du fichier.
  */
public class HelloWorld {

    /**
      * Affiche seulement "Hello World!" dans la console, car "Hi there!" est commenté.
      */
    public static void main(String[] args) {
        System.out.println("Hello World !");
        // System.out.println("Hi there !");

    }
}
```  
{% endmethod %}
