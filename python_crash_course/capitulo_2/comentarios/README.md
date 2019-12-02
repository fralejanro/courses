# Comentarios

En Python existen 3 tipos de comentarios de una sola línea, multilínea y comentarios de documentación (Docstring).

## Comentarios de un sola línea

En Python el carácter de numeral `#` indica un comentario de línea. Cualquier cosa que seiga después de un numeral será ignorada por el interprete de Python. Lo siguiente es un ejemplo de un comentario

```python
def suma(numero_1, numero_2):
	# retorna la suma de 2 números
	return numero_1 + numero_2
```

## Comentarios multilínea

Los comentarios multilínea sirven para describir o explicar el funcionamiento del programa, este tipo de comentarios debe comenzar con `"""` y terminar con `"""`. Cualquier cosa que este entre estos dos símbolos es ignorada por el compilador.  Lo siguiente es un ejemplo de un comentario multilínea.

```python
def suma(numero_1, numero_2):
	"""Función encargada de 
	    sumar dos números"""
	return numero_1 + numero_2
```

