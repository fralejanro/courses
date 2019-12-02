# Números

Los números se usan con bastante frecuencia en la programación. Python trata los números de diferentes formas. En este punto vamos a aprender sobre los enteros que son los más simples para trabajar en Python.

## Enteros

En Python se pueden sumar, restar, multiplicar y dividir enteros como se ve en el siguiente ejemplo.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 8 + 6
14
>>> 10 - 2
8
>>> 57 * 94
5358
>>> 20 / 2
10.0
```
### Exponentes

En Python la forma de representar exponentes es con dos simbolos de multiplicación como se ve en el siguiente ejemplo

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 2 ** 5
32
>>> 3 ** 3
27
```

## Flotantes

En Python cualquier número con un punto decimal se conoce como flotante. Con los flotantes se pueden realizar las mismas operaciones que con los enteros como se ve en el siguiente ejemplo.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 0.1 + 0.1
0.2
>>> 0.2 - 0.1
0.1
>>> 2 * 0.1
0.2
>>> 2 / 0.1
20.0
```

Algunas veces puede obtener un número arbitrario de decimales al realizar operaciones con flotantes y esto se debe a que Python intenta representar el resultado tan preciso como sea posible. Por ejemlo al sumar 0.1 + 0.2 se obtiene 17 decimales como se ve en el siguiente ejemplo.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 0.1 + 0.2
0.30000000000000004
```


## Guiones bajos en números

Cuando se escriben números de gran longitud, se pueden agrupar los dígitos usando guiones bajos para los números más legibles como se ve en el siguiente ejemplo.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> universe_age = 14_000_000_000
>>> print(universe_age)
14000000000
```

## Constantes

Una constante es una variable cuyo valor permanece igual durante toda la vida de un programa. Python no tiene tipos de constantes incorporadas pero para identificar las constantes el nombre de la variable se escribe todo en mayúsculas como se ve el siguiente ejemplo

```python
SPEED_SOUND = 343.2
```

