# Primitifs  
Les variables dites **primitives** sont des types de données simples que l'on retrouve dans presque tous les autres langages de programmation.
Elles peuvent être des nombres, un booléen ou un caractère Unicode.  
À partir de celles-ci, on crée d'autres variables : [**les objets**](objects.md).

Java possède [**8 primitive datatypes**](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html) par défaut. On les appelle les **Primitive Data Types** (ou juste Primitive).  

## Entiers  

| Type de variable | Définition | Minimum | Maximum | Valeur par défaut | Utilité |
| ---------------- | ----------- | ------- | ------- | ----------------- | ------- |
| byte | Un entier sur 8-bit signé (1 octet)| -128 (-2^7) | +127 (inclusif) (2^7 - 1) | 0 | byte est utilisé pour économiser de l'espace, principalement à la place des entiers, car un octet est quatre fois plus petit qu'un entier. |
| short | Un entier sur 16-bit signé (2 octets) | -32,768 (-2^15) | +32,767 (inclusif) (2^15 -1) | 0 | short est aussi utilisé pour économiser de l'espace. Il est deux fois plus petit qu'un entier. |
| int | Un entier sur 32-bit signé (4 octets)  | -2,147,483,648 (-2^31) | +2,147,483,647 (inclusif) (2^31 -1)  | 0  | int (Integer) est utilisé très généralement pour manipuler des entiers sans se soucier de la mémoire.  |
| long | Un entier sur 64-bit signé (8 octets)  | -9,223,372,036,854,775,808 (-2^63) | +9,223,372,036,854,775,807 (inclusif) (2^63 -1) | 0L  | long a la plus grande plage d'entiers possibles. Il est utilisé quand on a besoin d'entiers extrêmement grands. |  

{% method -%}
On voit que pour **certains types** de variables, on a besoin de spécifier le type avec une lettre derrière la valeur.  
Par défaut, un nombre est de type int. Nous devons donc spécifier à Java qu'il s'agit d'un autre type de variable. Pour cela, on va [convertir](cast.md) les objets.
{% sample lang="java" -%}
```java
byte b = (byte) 12; // On convertit le nombre en byte
short s = (short) 32_000; // De même en short
int i = 235_000; // On définit un entier normal
long l = 372_036_854_775_800L;// On spécifie le type long (grand nombre). Sans L, le code ne compilera pas.
// Note: Il est préférable d'utiliser des _ pour écrire de grands nombres.
```
{% endmethod %}

## Nombres réels

| Type de variable | Définition | Minimum | Maximum | Valeur par défaut | Utilité |
| ---------------- | ----------- | ------- | ------- | ----------------- | ------- |
| float | Un nombre réel simple avec une [précision simple](https://en.wikipedia.org/wiki/Single-precision_floating-point_format) sur 32-bits [IEEE 754 floating point](https://en.wikipedia.org/wiki/Single-precision_floating-point_format#IEEE_754_single-precision_binary_floating-point_format:_binary32)| Na | | Na | 0.0f | float est utilisé pour des calculs ne nécessitant pas une très grande précision comme la division. Il permet aussi d'économiser de l'espace comparé à double. |
| double | Un nombre réel double avec une [précision double](https://en.wikipedia.org/wiki/Single-precision_floating-point_format) sur 64-bits [IEEE 754 floating point](https://en.wikipedia.org/wiki/Double-precision_floating-point_format#IEEE_754_double-precision_binary_floating-point_format:_binary64)| Na | | Na | 0.0d | double est utilisé pour des calculs nécessitant une grande précision. Il souvent le choix par défaut. |

{% method -%}
{% sample lang="java" -%}
```java
float f = 1.0F; // On spécifie le type float
double d = 1.0D; // De même avec double
```
{% endmethod %}

## Autres  

| Type de variable | Définition | Minimum | Maximum | Valeur par défaut | Utilité |
| ---------------- | ----------- | ------- | ------- | ----------------- | ------- |
| boolean | Une information sur 1 bit. Accepte uniquement **true** ou **false** | Na | Na | false | boolean est utilisé pour stocker un état logique. |
| char | Un caractère Unicode 16-bit. | '\u0000' (ou 0) | '\uffff' (ou 65,535) | Na | char est utilisé pour stocker n'importe quel caractère (lettres, chiffres, % ou encore ❤). |  

{% method -%}
{% sample lang="java" -%}
```java
boolean b = true; // Une variable boolean
char c = '❤'; // Un caractère avec un coeur
```
{% endmethod %}
