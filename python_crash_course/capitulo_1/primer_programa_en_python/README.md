# Primer programa en Python

Si vienes de un lenguaje de programación como Java o C# lo más seguro es que esperes encontrar una función principal llamada `main()` que ejecute tu programa. Sin embargo, en Python no hay una función principal que se ejecute automaticamente, por lo cual podrás crear un archivo fuente que termine en la extensión .py y en el escribir las siguiente líneas

```python
print("Primer programa en Python")
```

con eso ya tendrás tu primer programa en Python que imprime por consola "Primer programa en Python". Ahora para ejecutarlo solo debes abrir tu terminal y escribir `python` seguido del nombre de tu archivo fuente.

```sh
$ python primer_programa.py
Primer programa en Python
```

Ahora bien si quieres definir una función `main()` primero debes saber algo, cada vez que el interprete de Python lee un archivo fuente hace dos cosas, establece algunas variables especiales como `__name__`, y luego ejecuta todo el código encontrado en el archivo.

Ahora veamos como funciona esto. Supongamos que tenemos el archivo primer_programa.py

```python
print("Hola mundo")

def main():
	print("Tienes una función main")

if __name__ == '__main__':
	main()

print("Adiós")
```

Primero el interprete define algunas variables especiales, en este caso nos vamos a centrar en la variable `__name__`, el interprete al iniciar le asigna el valor de `__main__` a la variable especial `__name__`.

```python
__name__ = "__main__"
```

Segundo el interprete sigue leyendo línea por línea del código e imprime "Hola mundo".

Tercero el interprete entra a la condición y al ser verdedara ejecuta la función `main()` e imprime "Tienes una función main".

Finamente lee la última línea e imprime "Adiós".

Tenga en cuenta que esto funciona de esta manera si esta ejecutando el archivo primer_programa.py como módulo principal, ya que si lo esta importando a la variable especial `__name__` se le asignara como valor el nombre de su archivo.

```python
__name__ = "primer_programa"
```
