# Estructuras de control

Las estructuras de control en Java se pueden agrupar en las siguientes categorías: selección, iteración y salto.

## Estructuras de selección 

Las estructuras de selección permiten que su programa se ejecute de acuerdo con los resultados de una expresión o con el estado de una variable. Java admite dos tipos de estructuras de selección: `if` y `switch`. 

### if 

La declaración if es la estructura utilizada para evaluar condiciones en Java. Puede ser utilizado por dos caminos diferentes. Aquí está la forma general de la declaración `if`

```sh
if (condición){
	sentencia1;
}else{
	sentencia2;
}
```

Aquí la declaración puede ser una declaración única o compuesta encerrada entre llaves(es decir, un bloque). La condición es cualquier expresión que devuelve un valor booleano. La cláusula `else` es opcional. Si la condición es verdadera se ejecuta la sentencia1, de lo contrario se ejecuta la sentencia2(si existe).

### if anidado

Un `if` anidado es una declaración `if` que contiene a otras declaraciones`if` o `else` dentro de su bloque. Lo siguiente es un ejemplo de un `if` anidado.

```java
int edad = 22;
if(edad > 18){
	if(edad > 21){
		System.out.println("Es mayor de edad en todos los paises");
	}else{
		System.out.println("Es mayor de edad en algunos paises");
	}
}else{
	System.out.println("Es menor de edad");
}
```

### Secuencia de ifs anidados

En muchas ocasiones va a necesitar utilizar una secuencia de ifs anidados para lo cual Java le provee una declaración conocida como escalera if-else-if que se ve de la siguiente manera:

```sh
if(condición){
	sentencia1;
}else if(condición){
	sentencia2;
}else if(condicion){
	sentencia3;
}else{
	sentenci0a4;
}
```

### switch

La declaración `switch` es una estructura de selección que le permite enviar la ejecución a diferentes partes de su código en función del valor de una expresión. Lo siguiente es la forma general de una declaración `switch`:

```sh
switch(expresión){
	case valor1:{
		// secuencia 1
		break;
	}
	case valor2:{
		// secuencia 2
		break;
	}
	case valor3:{
		// secuencia 3
		break;
	}
	case valor4:
	case valor5:{
		// secuencia 4
		// secuencia 5
		break;
	}
	case valorN:{
		// secuencia N
		break;
	}
	default:{
		/* secuencia que se ejecuta si el valor de la expresión 
		 no coincide con ningún caso*/
	}
}
```
expresión debe ser una constante(como un valor literal). No se permiten valores de casos repetidos, es decir, no puede tener el caso valor1 dos veces. El tipo de la expresión debe ser compatible con el valor de los casos. Para que varios casos ejecuten lo mismo se agrupan como en el caso de valor4 y valor5. La declaración `switch` funciona así: el valor de la expresión se compara con cada uno de los casos, si se encuentra una coincidencia, se ejecuta el código del caso respectivo. Si ninguna de las constantes coincide con el valor de la expresión se ejecuta el caso predeterminado, si no hay caso predeterminado no se ejecuta ningún caso y continúa la ejecución del programa.

 

