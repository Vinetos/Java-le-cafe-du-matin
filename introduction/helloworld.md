## Hello World {#helloworld}

En informatique, **Hello world** (traduit littéralement par « bonjour le monde ») sont les mots écrits dans un programme informatique **simple** dont le but est d'en faire la **démonstration**.
Autrement dit, ce sera notre **tout premier programme** dont le but sera de nous dire bonjour !

Lancez IntelliJ et cliquez sur « **Create New Project** ».

![](assets/helloworld/startup-intellij.png)

Choisissez **Java** et cliquez sur **Next**.

![](assets/helloworld/step1.png)

Cliquez une nouvelle fois sur **Next** puis entrez un nom et un endroit pour sauvegarder votre projet. Je l'appelle pour ma part **HelloWorld**.

![](assets/helloworld/step2.png)

> **[danger] Attention**
>
> Il est important de noter que votre « **Project location** » **ne doit pas contenir** autre chose que **des lettres, des chiffres et des espaces**.
> Autrement cela pose quelques bugs à l'IDE.

Cliquez sur **Finish** et patientez le temps de chargement.

Une nouvelle fenêtre va s'ouvrir. Elle contient **la structure du projet** à gauche et **l'éditeur de texte** à droite.
Faites un **clique droit** sur le dossier bleu "src" et **créez une nouvelle classe**.

![](assets/helloworld/step3.png)

Entrez « **HelloWorld** » comme nom et vérifiez que le type soit bien **Class**.

![](assets/helloworld/step4.png)

#### HelloWorld.java
Dans **l'éditeur de texte** (à droite), remplacez tout le contenu par celui-ci:

Votre fichier doit ressembler à ceci:

{% method -%}
![](assets/helloworld/step5.png)

{% sample lang="java" -%}
```java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello World !");
    }

}
```
{% endmethod %}

Cliquez sur la petite flèche verte à gauche du numéro des lignes et séléctionnez « **Run 'HelloWorld.main()'** ».

![](assets/helloworld/step6.png)

### Sortie console
Une fenêtre s'ouvre en bas et vous affiche « Hello World ! ».

![](assets/helloworld/step7.png)  

> **[success] Félicitations**
>
> **Félicitations**, vous venez de **créer, compiler et éxécuter** votre **premier** programme !
