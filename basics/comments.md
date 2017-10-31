# Les commentaires  

Les commentaires sont des lignes dans notre code qui vont être ignorées lors de la compilation et l'exécution du programme.  
Ils nous permettent d'expliquer des parties de codes compliquées. Ils sont utiles voir indispensables dès lors que l'on travaille en équipe, afin de faciliter la compréhension du code.

#### Regular comments

Il existe deux types de commentaires dits *réguliers* :  
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


#### La javadoc  
{% method -%}
La javadoc sert directement à la compréhension du code, que ce soit via l'inspection au sein d'un IDE, ou alors via un site web. Celui ci est généré à partir des sources d'un projet. La javadoc est un bloc spécifique de commentaires, que l'on initie avec deux **.En voici un exemple :  
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
Les commentaires s'utilisent n'importe où dans le code :  
{% sample lang="java" -%}
```java
package foo;

/*
 * Ce commentaire est généralement appelé "header" du fichier.
 */
public class HelloWorld {

    /**
     * Affiche seulement "Hello World!" dans la console, car "Hi there!" est commenté.
     */
    public static void main(String[] args) {
        System.out.println("Hello World !");
        // System.out.println("Hi there !");

        /* Ce commentaire contient d'autres messages qui sont ignorés
        System.out.println("Bonjour !");
        System.out.println("Salut ! ");
        */
    }
}
```  
{% endmethod %}
