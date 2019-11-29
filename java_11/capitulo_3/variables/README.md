# Variables

Las variables son la unidad básica de almacenamiento en un programa Java. Se define una variable por la combinación de un identificador, un tipo y un inicializador opcional. Todas las variables tienen un alcance, que define su visibilidad y una vida útil.

## Declaración de una variable

En Java todas las variables deben declararse antes de que puedan usarse. La forma básica de una declaración es así:

` tipo identificador [ = valor ][, identificador [= valor] ...];`

- tipo: Se refiere a uno de lo tipos atómicos de Java ya sea el nombre de una clase o de una interfaz.
- identificador:  Se refiere al nombre de la variable

Puede inicializar la variable especificando un signo `=` y un valor. Para declarar más de una variable del tipo especificado use una lista separada por comas.

Aquí hay varios ejemplos de declaraciones de variables.

```java
int age, weight, width;

double radio = 100.50,  pi = 3.14159;

char genre = 'F';
```

# Alcance y vida útil de las variables

Cada vez que comienza un nuevo bloque está creando un nuevo ámbito. Un ambito determina qué objetos son visibles para otras partes de su programa, también determina la vida útil de esos objetos. En Java los dos ámbitos principales son los definidos por una clase y los definidos por un método. El alcance definido por un método comienza con su llave de apertura `{`, si ese método tiene parámetros también se incluyen dentro del alcance del método. El alcance del método termina con su llave de cierre `}`. Como regla general las variables que declara dentro de un método no son visibles, es decir, accesibles fuera de ese ambito. 

