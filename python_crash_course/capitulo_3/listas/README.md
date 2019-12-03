# Listas

## ¿Qué es una lista?

Una lista es una colección de objetos en un orden en particular. Una lista puede contener cualquier tipo de objetos. En Python los corchetes `[]` indican una lista y los elementos individuales en la lista están separados por comas. Lo siguiente es un ejemplo de una lista que contiene algunas marcas de bicicletas:

```python
marcas_bicicletas = ["trek", "GW", "cannondale", "specialized"]
```

## Acceder a los elementos de una lista

Las listas son colecciones ordenadas, por lo que Python puede acceder a cualquiere elemento en la posición o índice deseado. Para acceder a un elemento de la lista se debe escribir el nombre de la lista seguido del índice del elemento entre corchetes. Por ejemplo saquemos el último elemento de la lista de marcas de bicicletas:

```python
marca_bicicleta = marcas_bicicletas[0]
```

Esto `marcas_bicicletas[0]` retorna el primer elemento de la lista de marcas de bicicletas. Se preguntará por qué en el índice aparece 0 y no 1, esto es porque Python considera que el primer elemento de una lista es el que se encuentre en el índice 0, esto es cierto para la mayoría de los lenguajes de programación.

## Acceder al último elemento de una lista

Python tiene una sintaxis especial para acceder al último elemento de una lista. Al acceder al índice `-1` Python siempre devuelve el último elemento de la lista. Por ejemplo saquemos el último elemento de la lista de marcas de bicicletas:

```python
marca_bicicleta = marcas_bicicletas[-1]
```

## Modificar elementos de una lista

La sintaxis para modificar un elemento de una lista es similar a la sintaxis para acceder a un elemento de una lista. Para modificar un elemento de una lista primero escriba el nombre de la lista seguido del índice del elemento que desea modificar entre corchetes, luego escriba el signo `=` y asignele el valor que desea. Por ejemplo vamos a cambiar la primera marca que aparece en la lista de marcas de bicicletas:

```python
marcas_bicicletas[0] = "giant"
```

Con lo anterior la primera marca ya no será  "trek" si no "giant".

## Agregar elementos a una lista

Python proporciona varias formas de agregar nuevos elementos a una lista.

### Agregar elemento al final de la lista

Para agregar un elemento al final de la lista se utiliza la función `append()` que recibe como parámetro el elemento que se va a agregar a la lista. Por ejemplo vamos a agregar un nuevo elemento a la lista de marcas de bicicletas:

```python
marca = "scott"
marcas_bicicletas.append(marca)
```

### Agregar elemento en una posición específica de la lista

Para agregar un elemento en una posición específica de la lista se utiliza la función `insert()` que recibe dos parámetros el primero es el índice donde desea agregar el elemento y el segundo es el elemento que desea agregar. Por ejemplo vamos a agregar un nuevo elemento en el índice 3 de la lista de marcas de bicicletas:

```python
marca = "orbea"
marcas_bicicletas.insert(3,marca)
```

## Eliminar elementos de una lista

Python proporciona varias formas de eliminar un elemento de una lista ya sea por su valor o por su índice.

### Eliminar el primer elemento de una lista por su valor

Para eliminar el primer elemento de una lista por su var se utiliza la función `remove()` que recibe como parámetro el valor del elemento que desea eliminar. Si el elemento no existe se lanza una excepción `ValueError`. Por ejemplo vamos a eliminar de la lista de marcas de bicicletas la marca "orbea"

```python
marcas_bicicletas.remove("orbea")
```
En caso de que existieran varias marcas con el mismo nombre esta función solo elimina la primera que coincida con el valor.

### Eliminar elemento de una lista en un índice específico.

Para eliminar un elemento de una lista en un índice específico se utiliza la función `pop()` que recibe como parámetro el índice del elemento que desea eliminar y al eliminarlo retorna el elemento eliminado. Por ejemplo vamos a eliminar de la lista de marcas de bicicletas el elemento que se encuentra en el índice 2. 

```python
 marca_eliminada = marcas_bicicletas.pop(2)
```
Tenga en cuenta que la función `pop()` también le permite eliminar el último elemento de la una lista cuando no le especifica ningún índice. En caso de que la lista este vacía se lanzara una excepción `IndexError`

### Eliminar un segmento de elementos de una lista

Para eliminar un segmento de elementos de una lista se utiliza la declaración `del` acomapañada del segmento de elementos a eliminar. Por ejemplo vamos a eliminar los elementos que se encuentran desde el índice 2 hasta el índice 4 de la lista de marcas de bicicletas:

```python
del marcas_bicicletas[2:4]
```

Tenga en cuenta que la declaración `del` no retorna los elementos eliminados y que también se puede utilizar para eliminar uno o todos los elementos.

## Invertir una lista

Para invertir una lista se utiliza la función `reverse()` que invirte el orden de los elementos, es decir el primer elemento será el último y así sucesivamente. Por ejemplo invirtamos la lista de marcas de bicicletas:

```python
marcas_bicicletas.reverse()
```


## Tamaño de una lista

Para obtener el tamaño de una lista se utiliza la función `len()` que recibe como parámetro la lista a la que se le desea obtener el tamaño y que retorna el tamaño de la lista.
Por ejemplo obtengamos el tamaño de la lista de marcas de bicicletas:

```python
numero_marcas = len(marcas_bicicletas)
```
