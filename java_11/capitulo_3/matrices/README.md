# Matrices

Una matriz es un grupo de variables del mismo tipo que se refieren a un nombre en común. Se pueden crear matrices de cualquier tipo y pueden tener una o más dimensiones. Para acceder a un elemento especifico en un matriz se utiliza su índice. 

## Matriz unidimensional

Una matriz unidimensional es esencialmente una lista de variables del mismo tipo. Para crear una matriz primero se debe crear una variable de matriz del tipo deseado. La forma general de una declación de matriz unidimensional es la siguiente:

`tipo identificador [];`
`tipo [] identificador;`

El tipo se refiere al tipo de datos de cada elemento que va a contener la matriz, el identificador se refiere al nombre de la matriz. Por ejemplo, lo siguiente declara una matriz de enteros.

```java
int [] monthDays;
```

Aunque esta declaración establece el hecho de que `monthDays` es una matriz, en realidad no existe una matriz. Para vincular a `monthDays` con una matriz física real de enteros se debe asignar una usando el operador `new` que es un comando especial que asigna memoria. La forma general de asignar memoria a una matriz es la siguiente:

`identificador = new tipo [tamaño];`

 Como se dijo anteriormente `new` asigna un espacio en memoria, tipo se refiere a los tipos de datos que se asignan a esa matriz y tamaño especifica el número de elemenetos que va a contener la matriz. Tenga en cuenta que una matriz no es dinámica por lo cual no puede cambiar su tamaño. Lo siguiente asigna una matriz de enteros de 8 elementos y los vincula a `monthDays`.

 `monthDays = new int [12];`

Después de que se ejecute la instrucción anterior `monthDays` será una matriz de 12 enteros. Además todos los elementos de la matríz se inicializarán en cero. Por otra parte todos los indices de la matrices comienzan en cero. Por ejemplo la siguiente instrucción asigna el valor de 12 al último elemento de la matriz `monthDays`

```java
monthDays[11] = 12;
```

Después de esto su matríz luciria así.

```sh
[0][0][0][0][0][0][0][0][0][0][0][12]
```

## Matriz multidimensional

En Java las matrices multidimensionales se implementan como matrices de matrices. Para declarar una variable de una matriz multidimensional se debe especificar cada indice adicional utilizando otro conjunto de corchetes. La forma general de una declación de matriz multidimensional es la siguiente:

`tipo identificador [] [];`
`tipo [][] identificador;`


 Por ejemplo lo siguiente declara e inicializa una variable de una matriz bidimensional de 10 filas y 5 columnas llamada weight.

```java
int [] [] weight = new int[10][5];
```

## Métodos y atributos para trabajar con matrices

Los siguientes métodos y atributos se pueden utilizar tanto en matrices unidimensionales como en matrices multidimensionales.

### Tamaño de una matriz

Las matrices tienen una variable llamada `length` que indica el tamaño de esa matriz. Al acceder a ella puede conocer el tamaño de su matriz.
El siguiente código imprime el tamaño de 2 matrices.

```java
// Matrices unidimensionales
int dogs [] = new int [10];
int cats [][] = new int [5][5];

System.out.println("Tamaño matriz dogs: "+ dogs.length + " tamaño filas matriz cats: "+ cats.length + " tamaño columnas matriz cats "+ cats[0].length);
```

### Clonar una matriz

Las matrices tienen un método llamado `clone()` que sirve para crear una copia exacta de una matriz. El siguiente código clona la matriz dogs y se la asigna a la variable animals.

```java
String dogs [] = {"pug", "german shepherd"};
String animals [] = dogs.clone();
``` 