# Les commentaires  

Les commentaires sont des lignes dans notre code qui vont être ignorée lors de la compilation et l'éxecution du programmes.  
Ils nous permettent d'expliquer des parties de codes compliqués. Ils ont utiles pour nous et les autres développeurs.

#### Regular comments

Il existe deux types de commentaires dits « **réguliers** » :  
{% method -%}
Des **Single-line** :  
```
// Ce commentaire ne couvre qu'une ligne et ignore tout ce qui se trouve jusqu'au prochain retour à la ligne.
```  

Des blocs de commentaires :  
```
/* Ce commentaire couvrent tout ce qui
   se trouve jusqu'ici */
```  

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

#### La javadocs

# Utiliser les commentaires
