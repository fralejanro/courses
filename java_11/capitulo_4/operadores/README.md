## Operadores

Java tiene un entorno rico en operadores. La mayoría de sus operadores se pueden dividir en los siguientes grupos: aritméticos, bit a bit(bitwise), relacionalees, lógicos, asignación, ternarios y de instancia.

### Aritméticos

Los operadores aritméticos se usan en expresiones matemáticas de la misma manera que se usan en álgebra. La siguiente tabla enumera los operadores aritméticos.

| Operador | Resultado |
| ------ | ------ |
| + | Suma |
| - | Resta |
| * | Multiplicación |
| / | División |
| % | Módulo |
| ++ | Incremento |
| -- | Decremento |
| += | Suma y asigna un valor a una variable |
| -= | Resta y asigna un valor a una variable  |
| *= | Multiplica y asigna un valor a una variable |
| /= | Divide y asigna un valor a una variable |
| %= | Modula y asigna un valor a una variable |

### Bit a bit(Bitwise)

Los operadores bit a bit se pueden aplicar a los tipos `long`, `int`, `short`, `char` y `byte`. Estos operadores actúan sobre los bits individuales de sus operandos. La siguiente tabla enumera los operadores bit a bit.

| Operador | Resultado |
| ------ | ------ |
| ~ | NOT bit a bit |
| & | AND bit a bit |
| &#124; | OR bit a bit |
| ^ | OR exclusivo bit a bit |
| &#62;&#62; | Desplazamiento a la derecha |
| &#62;&#62;&#62; | Desplazamiento a la derecha relleno cero |
| << | Desplazamiento a la izquierda |
| &= | AND y asignación bit a bit |
| &#124;= | OR y asignación bit a bit  |
| ^= | OR exclusivo y asignación bit a bit |
| &#62;&#62;&#61; | Desplazamiento a la derecha y asignación |
| &#62;&#62;&#62;&#61; | Desplazamiento a la derecha relleno cero y asignación |
| <<= | Desplazamiento a la izquierda y asignación |

### Relacionales

Los operadores relaciones determinan la relación que tiene un operando con el otro. La siguiente tabla enumera los operadores relacionales.

| Operador | Resultado |
| ------ | ------ |
| == | Igual a |
| != | Diferente de |
| > | Mayor que |
| < | Menor que |
| &#62;= | Mayor o igual |
| <= | Menor o igual |

### Lógicos

Los operadores lógicos solo operan en operandos booleanos. Todos los operadores lógicos binarios combinan dos valores booleanos para formar un valor booleano resultante. La siguiente tabla enumera los operadores lógicos.

| Operador | Resultado |
| ------ | ------ |
| & | Operación lógica AND |
| &#124; | Operación lógica OR |
| ^ | Operación lógica XOR |
| &#124;&#124; | Cortocircuito OR (Short-circuit OR) |
| && | Cortocircuito AND (Short-circuit AND) |
| ! | Operación lógica NOT |
| &= | Asignación AND |
| &#124;= | Asignación OR |
| ^= | Asignación XOR |
| == | Igual que |
| != | Diferente que |
| ?: | Operación ternaria si, entonces, de lo contrario |

Los operadores de cortocircuito `&&` y `||` no evaluán el lado derecho si no es necesario y los operadores `|` y `&` siempre evalúan ambos lados. Generalmente se usan los operadores de cortocircuito.

### Asignación

El operador de asignación es el signo `=`. Se utiliza para asignar un valor a cualquier variable. Su forma de asociar es de derecha izquierda, es decir, el valor establecido en el lado derecho se le asigna a la variable de la izquierda.

Su forma general es `variable = valor;`

### Ternarios

El operador ternario es un operador especial de tres vías que puede reemplazar ciertas declaraciones if-then-else. 

Su forma general es `expresion1 ? expresion2 : expresion3;`

Aquí la `expresion1` es cualquier expresión que se evalúe como un valor booleano. Si la `èxpresion1` es verdadera se evalúa la `expresion2` de lo contrario, se evalúa la `expresion3`.

### Instancia

El operador `instanceof` permite conocer el tipo de un objeto durante el tiempo de ejecución. El operador `instanceof`tiene esta forma general

`objref instanceof type`

Si `objref` es del tipo especificado o se puede convertir en el tipo especificado el operador `instanceof` se evalúa como verdadero, de lo contrario su resultado es falso.
