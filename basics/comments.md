# Les commentaires  

Les commentaires sont des lignes dans notre code qui vont être ignorée lors de la compilation et l'éxecution du programmes.  
Ils nous permettent d'expliquer des parties de codes compliqués. Ils ont utiles pour nous et les autres développeurs.

#### Regular comments

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
Un certain type de blocs de commentaires sont utilisés pour créer la **javadocs**. Pour faire simple, il s'agit de créer des pages html expliquant comment le code fonctionne. Nous reverrons cela plus tard.
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
Les commentaires s'utilisent n'importe où dans le code. Vous pouvez réaliser des choses comme cecis :  
{% sample lang="java" -%}
```java
public class HelloWorld {

    public static void main(String[] args) {
        // Permet d'afficher Hello World ! dans la console et de ne pas éxecuter Hi there !.
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
