# **Lenguaje de programacion Python** #

## Estructuras repetitivas ##

## *La sentencia for* ##

La sentencia for en Python difiere un poco de lo que uno puede estar acostumbrado en lenguajes como
C o Pascal. En lugar de siempre iterar sobre una progresión aritmética de números (como en Pascal) o
darle al usuario la posibilidad de definir tanto el paso de la iteración como la condición de fin (como en C),
la sentencia for de Python itera sobre los ítems de cualquier secuencia (una lista o una cadena de
texto), en el orden que aparecen en la secuencia. En cada iteración, el elemento siguiente del iterable se asigna al nombre de variable especificado:

    lista = ["a", "b", "c"]
    for i in lista: # Iteramos sobre una lista, que es iterable
    	print i

*a*

*b*

*c*

	cadena = "abcdef"

	for i in cadena:  Iteramos sobre una cadena, que también es iterable
		print i,   //añadiendo una coma al final hacemos que no introduzca un salto de línea, sino un espacio
    
*a b c d e f*
## *La sentencia while* ##

El bucle while evalúa una condición y, si es verdadera, ejecuta el bloque de código interno. Continúa evaluando y ejecutando mientras la condición sea verdadera. Se define con la palabra clave while seguida de la condición, y a continuación el bloque de código interno:

    >>> numero = 0
    >>> while numero < 10:
    ...     print numero,
    ...     numero += 1  #un buen programador modificará las variables de control al finalizar el ciclo while
    ...
    0 1 2 3 4 5 6 7 8 9

## *Variables* ##

Las variables se definen de forma dinámica, lo que significa que no se tiene que especificar cuál es su tipo de antemano y puede tomar distintos valores en otro momento, incluso de un tipo diferente al que tenía previamente. Se usa el símbolo = para asignar valores.

    x = 1
    x = "texto" # Esto es posible porque los tipos son asignados dinámicamente

## *Tipos de datos* ##
						      
**str**
-
	- Cadena
	- Inmutable	                                                   'Cadena'

**unicode**
-
	- Cadena
	- Versión Unicode de str	                                    u'Cadena'

**list**
-
	- Secuencia
	- Mutable, puede contener objetos de diversos tipos	            [4.0, 'Cadena', True]

**tuple**
-
	- Secuencia
	- Inmutable, puede contener objetos de diversos tipos	        (4.0, 'Cadena', True)

**set**
-
	- Conjunt
	- Mutable, sin orden, no contiene duplicados	                 set([4.0, 'Cadena', True])

**frozenset**
-
	- Conjunto
	- Inmutable, sin orden, no contiene duplicados	                 frozenset([4.0, 'Cadena', True])

**dict**
-
	- Mapping
	- Grupo de pares clave:valor	                                 {'key1': 1.0, 'key2': False}

**int**
-
	- Número entero
	- Precisión fija, convertido en long en caso de overflow.	     42

**long**
-
	- Número entero
	- Precisión arbitraria	                                         42L ó 456966786151987643L

**float**
-
	- Número decimal
	- Coma flotante de doble precisión	                             3.1415927
	
**complex**
-
	- Número complejo
	- Parte real y parte imaginaria j.	                             (4.5 + 3j)

**bool**
-
	- Booleano
	- Valor booleano verdadero o falso                               True o False

##*Definicion de funciones* ##

Las funciones se definen con la palabra clave def, seguida del nombre de la función y sus parámetros. Otra forma de escribir funciones, aunque menos utilizada, es con la palabra clave lambda (que aparece en lenguajes funcionales como Lisp).
El valor devuelto en las funciones con def será el dado con la instrucción return.

def:

    >>> def suma(x, y = 2):
    ...     return x + y # Retornar la suma del valor de la variable "x" y el valor de "y"
    ...
    >>> suma(4) # La variable "y" no se modifica, siendo su valor: 2
    6
    >>> suma(4, 10) # La variable "y" sí se modifica, siendo su nuevo valor: 10
    14

lambda:

    >>> suma = lambda x, y = 2: x + y
    >>> suma(4) # La variable "y" no se modifica, siendo su valor: 2
    6
    >>> suma(4, 10) # La variable "y" sí se modifica, siendo su nuevo valor: 10
    14