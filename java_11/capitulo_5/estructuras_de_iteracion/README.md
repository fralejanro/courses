# Estructuras de iteración

Las estructuras de iteración en Java son `for`, `while` y `do-while`. Estas estructuras comunmente se conocen como bucles. Un bucle ejecuta repetidamente el mismo conjunto de instrucciones hasta que se cumpla una condición de terminación.


## while

El bucle `while` es la estructura de iteración más fundamental en Java. Repite una declaración mientras su expresión de control sea verdadera. Lo siguiente es su forma general:

```sh
while(condición){
	//instrucciones
}
```

La condición puede ser cualquier expresión booleana. Las instrucciones serán ejecutadas siempre que la condición sea verdadera si la condición es falsa nunca se ejecutarán las instrucciones dentro del cuerpo del bucle. Cuando la condición se convierte en falsa, el control pasa a la siguiente línea de código que sigue inmediatamente al bucle. El cuerpo de un bucle while puede estar vacío. Esto es porque una delación nula(una que consiste solo en un punto y coma) es sintácticamente válida en Java. Lo siguiente es un bucle while con un cuerpo vacío:

```java
 int i, j;

 i = 100;
 j = 200;

 while(+++i < --j);
 ```

 ## do-while

El bucle `do-while` a diferencia del bucle `while` siempre se ejecutará al menos una vez ya que la expresión condicional que controla el bucle se ejecuta en la parte inferior del bucle y no en el inicio. Lo siguiente es su forma general:

```sh
do {
	// instrucciones
} while(condición);
```

Cada iteración del bucle `do-while` ejecuta primero el cuerpo del bucle y luego evalúa la expresión condicional. Si esta expresión es verdadera el bucle se repite, de lo contrario el bucle termina. Como en todos los bucles de Java la condición debe ser una expresión booleana.

## for

El bucle `for` es un poco más sofisticado que los bucles `while` y `do-while`. Lo siguiente en su forma general:

```sh
for(inicialización; condición; iteración){
	// instrucciones
}
```

Cuando el bucle `for` inicia por primera vez lo primero que se ejecuta es la parte de inicialización del bucle. Generalmente esta es una expresión que establece el valor de las variables de control del bucle. Luego se evalúa la condición. Ésta debe ser una expresión booleana. Finalmente se ejecuta la parte de iteración que usualmente es una expresión que incrementa o disminuye la variable de control del bucle. Luego el bucle itera hasta que la expresión de la condición sea falsa. 

Java le permite incluir multiples declaraciones tanto en la parte de inicialización como en la parte de iteración. Esto es necesario para cuando el bucle es controlado por más de una variable. Lo siguiente es un ejemplo de un bucle `for` que es controlado por dos variables:


```java
for(int a=1, b=4; a<b; a++, b--){
	System.out.println("a = " + a);
	System.out.println("b = " + b);
}
```

El bucle `for` tiene dos variaciones que son poco utilizadas pero es bueno conocerlas. La primera variación es omitir las partes de declaración e iteración con el fin de utilizar solo la parte de la condición para controlar el bucle, esta variación se asemejaría a un bucle `while`. Lo siguiente es un ejemplo de la varación antes mencionada:

```java
boolean validation = true;
for( ; validation ; ){
	// instrucciones
}
```

La segunda variación es omitir las partes de declaración, condición e iteración esto con la intención de generar un bucle infinito como se ve en el siguiente ejemplo:

```java
for( ;  ; ){
	// instrucciones
}
```

## For-Each

Un bucle `for-each` esta diseñado para recorrer una colección de objetos de manera estrictamente secuencial, de principio a fin. Su forma general es la siguiente:

```sh
for(tipo variableIterar : colección){
	// instrucciones
}
```

Aquí el tipo especifica el tipo, variableIterar especifica el nombre de una variable que recibirá los elementos de una colección y colección especifica la colección que se va a recorrer.

