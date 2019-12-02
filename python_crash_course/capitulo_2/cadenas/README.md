# Cadenas

Las cadenas son una secuencia de caracteres que se encuentran dentro de unas comillas simples o dobles. Cualquier cosa entre comillas simples o dobles se consideran una cadena en Python. Lo siguiente son ejemplos de cadenas.

```sh
"Esto es una cadena"
'Esto también es una cadena'
```

## Algunas funciones para trabajar con cadenas

### Convertir el primer carácter de cada palabra en mayúsculas

Para convertir el primer carácter de cada palabra en mayúscula se utiliza la función `title()`.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> full_name = "stan lee"
>>> print(full_name.title())
Stan Lee
```

### Cambio de mayúsculas a minúsculas

Para converir todos los carácteres de una cada a minúsculas se utiliza la función `lower()`.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> full_name = "STAN LEE"
>>> print(full_name.title())
stan lee
```

### Cambio de minúsculas a mayúsculas

Para converir todos los carácteres de una cada a mayúsculas se utiliza la función `upper()`.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> full_name = "stan lee"
>>> print(full_name.title())
STAN LEE
```

## Usar variables en cadenas

En algunas ocasiones es necesario usar el valor de una variable dentro de una cadena. Por ejemplo, es posible que desee dos variables para representar un nombre y un apellido y luego combinar esas dos variables para mostrar el nombre completo de alguién. Para insertar el valor de una variable en un cadena, se debe colocar la letra `f` inmediatamente antes de la aparterue de las comillas, luego se debe poner llaves alrededor de cualquier variable que se desee usar dentro de la cadena. Python reemplazará cada variable con su valor cuando se muestre la cadena.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> first_name = "Roger"
>>> last_name = "Federer"
>>> full_name = f"{first_name} {last_name}"
>>> print(full_name)
Roger Federer
```

Estas cadenas se llaman cadenas `f`. La f es para el formato, porque Python formate la cadena para reemplazar el nombre de caulquier variable entre llaves con su valor. También puede utilizar las funciones al utilizar las variables dentro de las cadenas. Las cadenas `f` se introdujeron a partir de la versión Python 3.6.

## Agregar espacios en blanco a cadenas con tabuladores o nuevas líneas

### Agregar tabulador

Para agregar un tabulador a su texto, se debe usar la secuencia de escape `\t` como se muestra en el siguiente ejemplo

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> print("Python")
Python
>>> print("\tPython")
        Python
```

### Agregar una nueva línea

Para agregar una nueva línea a su texto, se debe usar la secuencia de escape `\n` como se muestra en el siguiente ejemplo

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> print("Languages:\nPtyhon\nJava\nRuby\nJavaScript")
Languages:
Ptyhon
Java
Ruby
JavaScript
```

## Eliminar espacios en blanco

Python puede buscar espacios en blanco en los lados derecho e izquierdo de una cadena o eliminar los espacios en ambos lados. 

### Eliminar espacios en blanco a la derecha

Para eliminar los espacios en blanco al lado derecho de una cadena se utiliza la función `rstrip()` como se ve en el siguiente ejemplo. Tenga en cuenta que esta función retorna una cadena sin los espacios en blanco a la derecha pero no asigna ese retorno a la variable.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> perro = "    pug"
>>> print(perro.rstrip())
    pug
```

### Eliminar espacios en blanco a la izquierda

Para eliminar los espacios en blanco al lado izquierdo de una cadena se utiliza la función `lstrip()` como se ve en el siguiente ejemplo. Tenga en cuenta que esta función retorna una cadena sin los espacios en blanco a la izquierda pero no asigna ese retorno a la variable.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> perro = "pug    "
>>> print(perro.lstrip())
    pug
```

### Eliminar espacios en blaco a ambos lados 

Para eliminar los espacios en blanco al lado derecho y al lado izquierdo de una cadena se utiliza la función `strip()` como se ve en el siguiente ejemplo. Tenga en cuenta que esta función retorna una cadena sin los espacios en blanco a lado derecho ni al lado izquierdo pero no asigna ese retorno a la variable.

```sh
$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
>>> perro = "    pug    "
>>> print(perro.strip())
    pug
```
