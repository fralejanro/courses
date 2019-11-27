# Léxico

Los programas escritos en Java son una colección de espacios en blanco, identificadores, literales, comentarios, operadores, separadores y palabras clave.

## Espacios en blanco

Java es un lenguaje de forma libre, es decir, no necesita seguir ninguna regla especial de sangría. Los espacios en blanco son los espacios, tabulación, una nueva línea y un avance de formulario (Form Feed).


## Identificadores

Los identificadores se usan para nombrar cosas como clases, variables y métodos. Un identificador puede ser cualquier secuencia de letras mayúsculas y minúsculas, números, guiones bajos. No deben comenzar con un número. Por convencción se utiliza el Camel Case pero para las constantes `static final` y para los valores de las enumeraciones se utiliza el Snake Case. Algunos ejemplos de identificadores válidos son:

- age
- fullName
- number1

## Comentarios

En Java hay tres tipos de comentarios que son comentarios de [una línea][2], [multilínea][1] y comentarios de documentación.


## Operadores

Java tiene un entorno rico en operadores. La mayoría de sus operadores se pueden dividir en los siguientes grupos: aritméticos, bit a bit(bitwise), relacionalees, lógicos, asignación, ternarios y de instancia.

## Separadores

En Java hay algunos caracteres que se usan como separadores. La siguiente tabla enumera los separadores.

| Separador | Uso |
| ------ | ------ |
| Paréntesis () | Usados para contener una lista de parámetros en la definición e invocación de un método. También se utilizan para definir la precedencia en operaciones, en sentencias de control y para envolver tipos de casteo.
| Llaves {} | Usados para contener una lista de parámetros en la definición e invocación de un método. También se utilizan para definir la precedencia en operaciones, en sentencias de control y para envolver tipos de casteo. |
| Corchetes [] | Usados para declarar tipos de matrices. También se utilizan para referenciar una posición dentro de una matriz. |
| Punto y Coma ; | Usado para terminar declaraciones |
| Punto . | Usado para separar nombres de paquetes subpaquetes y clases. También se utiliza para separar una variable o método de una variable de referencia. |
| Dos puntos seguidos :: | Usados para crear un método o para referencia un constructor. |
| Elipsis ... | Usado para indicar que un método recibe n variables. |
| Arroba @ | Usado para indicar el inicio de una anotación |

## Palabras clave

Actualmente hay 61 palabras claves definidas en Java. Las palabras claves no pueden usarse como nombres para una variable, clase o método. A partir del JDK9, un guión bajo se considera una palabra clave para evitar su uso como el nombre de algo en su programa.

| | | | | | |
| -| -| -| -| -| -|
| abstract | assert | boolean | break | byte | case |
| catch | char | class | const | continue | default |
| do | double | else | enum | exports | extends |
| final | finally | float | for | goto | if |
| implements | import | instanceof | int | interface | long |
| module | native | new | open | opens | package |
| private | protected | provides | public | requires | return |
| short | static | strictfp | super | switch | synchronized |
| this | throw | throws | to | transient | transitive |
| try | uses | void | volatile | while | with |
| _ |  |  |  |  |  |

Ademas de las palabras clave se reserva otro cuatro nombres. Tres han sido los valores `true`, `false` y `null`. La cuarta es la palabra `var` que se ha agregado a partir del JDK10.


[1]: <https://github.com/fralejanro/courses/tree/master/java_11/capitulo_2/primer_programa_en_java#comentario-multil%C3%ADnea>

[2]: <https://github.com/fralejanro/courses/tree/master/java_11/capitulo_2/primer_programa_en_java#comentario-de-una-sola-l%C3%ADnea>
