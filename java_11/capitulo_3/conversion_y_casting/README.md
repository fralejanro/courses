# Conversión Automática

La conversión automática entre dos tipos de datos tendrá lugar si se cumplen las siguientes dos condiciones:

- Los dos tipos son compatibles
- El tipo de destino es más grande que el tipo de origen

Por ejemplo el tipo `int` tiene un rango lo suficientemente grande para contener todos los valores de bytes válidos. por lo que no se requiere de una conversión explícita.


# Casting

Aunque las conversiones automáticas de tipos son útiles, no satisfacen todas las necesidad. Por ejemplo ¿Qué sucede si desea asignar un valor `int` a una variable de `byte`? Esta conversión no se realizará automáticamente, porque un `byte` es más pequeño que un `int`. Este tipo de conversión a veces se denomina conversión de reducción ya que explícitamente está reduciendo el valor para que se ajuste al tipo de destino.

La forma general de este tipo de conversión es la siguiente:

`(tipo objetivo)  valor`

El tipo objetivo especifica el tipo de dato al que desea convertir el valor especificado. Por ejemplo el siguiente fragmento de código convierte un int en un byte.

```java
int a;
byte b;
// ... 
b = (byte) a;
```