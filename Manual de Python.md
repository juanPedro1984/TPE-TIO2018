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

