# Primer programa en Java

A continuación vamos a mostrar la estructura básica de un programa en Java.

```java
/*
  Este es un ejemplo de un programa en java
*/

class PrimerPrograma{

	public static void main(String args[]){

		// Imprime por consola Primer programa en Java
		System.out.println("Primer Programa en Java");
	}
}
```

Lo primero que debes aprender sobre Java es que un archivo fuente oficialmente se conoce como una unidad de compilación, que básicamente es un archivo de texto que contiene una o más definiciones de clase y usa la extensión .java, por lo cual el nombre del archivo fuente debe ser igual al nombre de una de las clases definidas. En nuestro caso anterior el nombre del archivo fuente debe ser PrimerPrograma.java ya que solo tenemos definida una clase. También debe asegurarse que la capitalización del nombre del archivo fuente coincide con el nombre de la clase, esto debido a que Java distingue entre mayúsculas y minúsculas. La convención que se utiliza para el nombre de las clases es [PascalCase][1]. 

## Examinemos cada parte del programa

### Comentario multilínea

Nuestro primer programa empieza con las siguientes líneas

```java
/*
  Este es un ejemplo de un programa en java
*/
```
Esto es un comentario multilínea que sirve para describir o explicar el funcionamiento del programa, este tipo de comentarios debe comenzar con `/*` y terminar con `*/`. Cualquier cosa que este entre estos dos símbolos es ignorada por el compilador. 

### Declaración de la Clase

```java
class PrimerPrograma{
```
Esta línea usa la palabra clave `class` para declarar que se esta definiendo una nueva clase y PrimerPrograma es el identificador que es el nombre de la clase.


### Método main

```java
public static void main(String args[]){
```

Esta línea comienza el método main. Utiliza la palabra clave `public` que es un modificador de acceso, que permite que este método pueda llamarse fuera de su clase. La palabra clave `static` permite que se llame a `main()` sin tener que instanciar una instancia particular de la clase. La palabra clave `void` simplemente indica que el método `main()` no retorna ningún valor. La palabra main es el identificador que es el nombre del método. Ahora cualquier información que necesite pasar a un método es recibida por variables y son especificadas dentro del conjunto de paréntesis que siguen al nombre del método. Estas variables se llaman parámetros. Si no necesita incluir ningún parámetro debe incluir los paréntesis vacíos. Para nuestro caso 
`(String args[])`declara un parámetro de nombre args, que es un vector de objetos String. Esta llave de apertura `{`indica el inicio del cuerpo del método `main()`. Todo el código  que se encuentre entre la llave de apertura y la llave de cierre solo se ejecutará cuando el método `main()` sea llamado.

#### Comentario de una sola línea

```java
// Imprime por consola Primer programa en Java
```
Esta línea es un comentarío de línea que sirve para dar descripciones breves línea por línea.

#### Impresión por consola

```java
System.out.println("Primer Programa en Java");
```

Esta línea imprime por consola "Primer Programa en Java". Esta salida se logra utilizando el método `println()` que está incorporado en la clase `System` que proporciona acceso al sistema y `out` es el flujo de salida que está conectado a la consola.


[1]: <http://wiki.c2.com/?PascalCase>
