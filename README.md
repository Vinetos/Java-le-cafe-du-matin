# Java, le café du matin

_Java, le café du matin_ est un livre destiné à un **public débutant** en informatique voulant se lancer dans une **première expérience** de programmation. Il permettra d’**appréhender** les concepts de ce langage interplanétaire, d’en comprendre le **fonctionnement** et bien évidemment, d’**apprendre à écrire** vos premiers programmes.

Ce livre a une particularité : il est **open-source**. Libre à vous de contribuer à l’écriture de celui-ci et d'ajouter votre pierre à l'édifice sur [le projet GitHub](https://github.com/Vinetos/Java-le-cafe-du-matin).  
Il est lisible en ligne [ici](https://java.vinetos.fr).

Une version **PDF** du livre est téléchargeable [en cliquant ici](https://www.gitbook.com/download/pdf/book/vinetos/java-le-cafe-du-matin).

####  Note de mise à jour :
Ce livre écrit pour Java 8 est en cours d'amélioration pour Java 9 et 10.

##  L'auteur principal
Vinetos, ou Valentin de son vrai nom, est un jeune développeur informatique. Grand fan d'informatique et d’électronique, il « bricole et bidouille pleins de petits trucs » comme diraient ses parents. Il essaye un maximum de choses et expérimente tout et n'importe quoi. Il aime comprendre comment un système fonctionne (reverse-engeenering) et aime produire tout lui-même. « Logiciels, applications (mobile & web), graphisme, animations (2D et 3D), compositions musicales sont des choses que j'aime faire ! Ce livre est pour moi une façon de partager ma connaissance à ceux qui souhaite s'aventurer dans la même branche que moi. C'est pour moi une occasion de transmettre ma passion et mon expérience.».  

## À propos du cours
Ce cours est proposé avec des appuis vidéos dans le but d'aider la compréhension. N'hésitez donc pas à visiter la chaine YouTube.  
De plus, des sections d'**analogie** sont disponibles dans plusieurs parties du cours pour que puissiez comprendre de quoi en parle et ne pas rester bloqués. Elles se situent souvent en début ou fin de cours/chapitres (avec la conclusion).  

## Comment participer au livre
### Prérequis  

Ce livre utilise [GitBook](https://www.gitbook.com) pour la mise en forme et la publication. Pour participer à l'édition du livre, vous avez deux prérequis :
 * NodeJS (v4.0.0 et plus)
 * Windows, Linux, Unix, or Mac OS X

### Installation avec NPM

{% method -%}
La meilleure façon d'installer GitBook est via NPM. Ouvrez un terminal et tapez cette commande :
{% sample lang="bash" -%}
```bash
$ npm install gitbook-cli -g
```
{% endmethod %}

gitbook-cli est un utilitaire pour installer plusieurs versions de gitbook sur le même système.
Il permet, en autres, d'installer automatiquement la version de gitbook utilisé par le livre.

### Cloner le livre

Faites une copie du [projet GitHub](https://github.com/Vinetos/Java-le-cafe-du-matin) et ouvrez un terminal dans celui-ci.

{% method -%}
On initialise le projet avec :  

{% sample lang="bash" -%}
```bash
$ gitbook init
```
{% endmethod %}

Vous pouvez désormais éditer le livre.

### Afficher les modifications

Pour vérifier que vos corrections s'adaptent avec le livre, vous devez le tester en local.
{% method -%}
Installez les plugins du livre avec :  

{% sample lang="bash" -%}
```bash
$ gitbook install
```  
{% endmethod %}
{% method -%}
Ensuite, vous pouvez prévisualiser votre livre en temps réel avec :  

{% sample lang="bash" -%}
```bash
$ gitbook serve
```  
{% endmethod %}  

> **[info] Notes**
>
> Une fois lancé, **si vous modifiez un fichier**, il suffit de le **sauvegarder** et le navigateur **s'actualisera tout seul**.

{% method -%}
ou générer les pages du site avec :
{% sample lang="bash" -%}
```bash
$ gitbook build
```  
{% endmethod %}

### Soumettez

Si vous pensez que tout est correct, créez une pull request, les modifications seront revues et seront ajoutées dans le livre si elles sont retenues !  

### Contributeurs  
* Valentin Chassignol (**_Vinetos_**)
* Charles D. (**_Gogume1er_**)
* Valentin Burgaud (**_Xharos_**)

> _(C) 2017-2018 Vinetos - Tous droits réservés._
