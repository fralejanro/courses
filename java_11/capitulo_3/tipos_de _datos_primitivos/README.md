# Tipos de datos primitivos

Java define ocho tipos primitivos de datos: `byte`, `short`, `int`, `long`, `char`, `float`, `double` y `boolean`. Estos tipos de datos se pueden agrupar en cuatro grupos:

- Enteros: Son `byte`, `short`, `int` y `long`. Representan números con signo de valor entero.
- Números de coma flotante: Son `float` y `double`. Representan números con precisión fraccional.
- Caracteres: Son`char`. Representan símbolos en un conjunto de caracteres como letras y números.
- Booleano: Son `boolean`. Representan valores falsos o verdaderos.

 Los tipos de datos primitivos representan valores únicos, no objetos.

 ## Enteros

 Java define cuatro tipos de enteros: `byte`, `short`, `int` y `long` representan valores enteros positivos o negativos. Java no admite enteros sin signo, a menos de que sean positivos. El ancho y el rango que utilizan los enteros se especifican en la siguiente tabla.

 | Nombre | Ancho | Rango |
 | ------ | ------ | ------ |
 | long | 64 bits | -9,223,372,036,854,775,808 a 9,223,372,036,854,775,807 |
 | int | 32 bits | -2,147,483,648 a 2,147,483,647 |
 | short | 16 bits | -32,768 a 32,767 |
 | byte | 8 bits | -128 a 127 |

 ### byte

El tipo entero más pequeño es el `byte`. Este es un tipo de 8 bits que tiene un rango entre -128 a 127. Las variables de tipo byte son útiles cuando se trabaja con secuencias de datos de una red o un con archivos. Las variables de bytes se declaran mediante el uso de la palabra clave `byte`

Lo siguiente declara una valariable de bytes

```java
byte file;
```

### short

El tipo `short` es un tipo de 16 bits que tiene un rango entre -32,768 a 32,767. Es uno de los tipos de datos menos utilizado. Las variables de tipo `short` se declaran mediante el uso de la palabra clave `short`.

Lo siguiente declara una variable del tipo `short`

```java
short departments;
```

### int

El tipo entero más utilizado es el `int`. Este es un tipo de 32 bits que tiene un rango entre -2,147,483,648 a 2,147,483,647. Su principal uso es para controlar bucles y para indexar matrices. Las variables de tipo `int` se declaran mediante el uso de la palabra clave `int`.

Lo siguiente declara una variable del tipo `int`

```java
int age;
```

### long

El tipo `long` es un tipo de 64 bits que tiene un rango entre -9,223,372,036,854,775,808 a 9,223,372,036,854,775,807. Es util cuando un tipo `int` no es lo suficientemente grande para contener el valor deseado. Las variables de tipo `long` se declaran mediante el uso de la palabra clave `long`.

Lo siguiente declara una variable del tipo `long`

```java
long speedOfLight;
```

## Números de coma flotante

Java implementa el conjunto estadar (IEE - 754) de tipos y operadores de coma flotante. Hay dos tipos de coma flotante que son `float` y `double` que representan precisión simple y doble. El ancho y el rango que utilizan los números de coma flotante se especifican en la siguiente tabla.

 | Nombre | Ancho | Rango aproximado |
 | ------ | ------ | ------ |
 | double | 64 bits | 4.9e-324 a 1.8e+308 |
 | float | 32 bits | 1.4e-045 a 3.4+038 |

### float

El tipo `float` es un tipo de precisión simple que utiliza 32 bits de almacenamiento y tiene un rango aproximado entre 1.4e-045 a 3.4+038. La precisión simple es más rápida en algunos procesadores y ocupa la mitad de espacio que la precisión doble, sin embargo, se volverá imprecisa cuando los valores sean muy grandes o muy pequeños. Las variables de tipo `float` se declaran mediante el uso de la palabra clave `float`.

Lo siguiente declara una variable del tipo `float`

```java
float price;
```

### double

El tipo `double` es un tipo de precisión doble que utiliza 64 bits de almacenamiento y tiene un rango aproximando entre 4.9e-324 a 1.8e+308. La precisión doble en realidad es más rápida que la precisión simple en algunos procesadores modernos que han sido optimizados para cálculos matemáticos de alta velocidad. Todas las funciones matemáticas trascendentales como sen(), cos() y sqrt() devuelve valores del tipo `double`. Las variables de tipo `double` se declaran mediante el uso de la palabra clave `double`.

Lo siguiente declara una variable del tipo `double`

```java
double radius;
```

## Caracteres

El tipo de dato utilizado para almacenar caracteres es el `char`. Es un tipo que utiliza 16 bits y que tiene un rango entre 0 a 65,536. Las variables de tipo `char` se declaran mediante el uso de la palabra clave `char`.

Lo siguiente declara una variable del tipo `char`

```java
char arroba;
```

## Booleanos

El tipo de dato utilizado para almacenar valores lógicos es el `boolean`. Una variable del tipo `boolean` solo puede tener uno de dos valores posibles `true` o `false`. Las variables de tipo `boolean` se declaran mediante el uso de la palabra clave `boolean`.

Lo siguiente declara una variable del tipo `boolean`

```java
boolean submited;
```

