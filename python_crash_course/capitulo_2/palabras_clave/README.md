# Palabras clave

Cada una de las siguientes palabras clave tiene un significado específico, y verá un error si intenta usar alguna de ellas como nombre de una variable.

| | | | |
| ------ | ------ | ------ | ------ |
| False | class | from | or |
| None | continue | global | pass |
| True | def | if | raise |
| and | del | import | return |
| as | elif | in | try |
| assert | else | is | while |
| async | except | lambda | with |
| await | finally | nonlocal | yield |
| break | for | not |  |

Una forma de saber cuales son las palabras claves es ejecutar el siguiente comando desde el shell de python `help("keywords")` al ejecutarlo le retornara una lista con las palabras clave de la versión de Python que está usando.

```sh
~$ python
Python 3.7.4 (default, Sep  2 2019, 20:47:34) 
[GCC 7.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> help("keywords")

Here is a list of the Python keywords.  Enter any keyword to get more help.

False               class               from                or
None                continue            global              pass
True                def                 if                  raise
and                 del                 import              return
as                  elif                in                  try
assert              else                is                  while
async               except              lambda              with
await               finally             nonlocal            yield
break               for                 not                 
```