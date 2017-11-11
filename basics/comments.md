# Les commentaires  

Les commentaires sont des lignes dans notre code qui vont être ignorées lors de la compilation et l'exécution du programme.  
Ils nous permettent d'expliquer des parties de codes compliqués. Ils sont utiles pour nous et les autres développeurs.

#### Les commentaires réguliers

Il existe deux types de commentaires dits « **réguliers** » :  
{% method -%}
Des **Single-line** :  
{% sample lang="java" -%}
```
// Ce commentaire ne couvre qu'une ligne et ignore tout ce qui se trouve jusqu'au prochain retour à la ligne.
```  
{% endmethod %}
{% method -%}
Des blocs de commentaires :  
{% sample lang="java" -%}
```
/* Ce commentaire couvre tout ce qui
   se trouve jusqu'ici */
```  
{% endmethod %}


#### La javadocs  
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
Les commentaires s'utilisent n'importe où dans le code. Vous pouvez réaliser des choses comme ceci :  
{% sample lang="java" -%}
```java
public class HelloWorld /* Ma classe HelloWorld*/{

    public static void /*void car la fonction ne renvoie rien*/ main(String[] args) {// Ma méthode
        // Permet d'afficher Hello World ! dans la console et de ne pas éxecuter Hi there !.
        System.out.println("Hello World !"); // Fait l'action
        // System.out.println("Hi there !");

        /* Ce commentaire contient d'autres messages qui sont ignorés
        System.out.println("Bonjour !");
        System.out.println("Salut ! ");
        */
    }
}
```  
{% endmethod %}
