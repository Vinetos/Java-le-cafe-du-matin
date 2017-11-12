# Les classes
Comme vu précédemment, les classes sont les plans de chaque objet créé.
{% method -%}
Voici un exemple de classe :
{% sample lang="java" -%}
```java
public class Voiture {

  static final int vitessMaximum = 130;// 130 km/h (static car valable pour toutes les voitures
  // final car elles ne doit pas changer peut importe le moment)

  String couleur;// Rouge, bleue...
  int vitesse;// La vitesse actuelle de la voiture en mk/h

  /**
    * Méthode pour accélérer
    */
  void accelerer() {

  }

  /**
    * Méthode pour freiner
    */
  void freiner() {

  }

  /**
    * Méthode pour utiliser l'avertisseur sonore (PAS EN AGGLOMÉRATION sauf danger).
    */
  void klaxonner() {

  }

}
```
{% endmethod %}  

Une classe peut contenir les types d’attributs (variables) suivants :
* **Variables locales** : Les variables locales sont définies dans les méthodes, constructeurs ou des blocs. La variable sera déclarée et initialisée dans la méthode et sera détruite quand la méthode sera terminée.
* **Variables d’instance** : Les variables d’instance sont définies dans une classe, mais en dehors de toutes méthodes. Elles sont initialisées quand la classe est instanciée (quand on crée un objet, on instancie une classe). Les variables d'instance peuvent être accessibles depuis n'importe quelle méthode, constructeur ou blocs de cette classe particulière.
* **Variables de classes** : Les variables de classe sont déclarées dans une classe mais en dehors de n’importe méthode, constructeur ou bloc. Elles utilisent le mot-clé ``static``.
