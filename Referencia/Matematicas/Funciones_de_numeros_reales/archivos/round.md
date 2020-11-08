# round

Redondea un número al entero más cercano.

## Sintaxis

  
```gml  
round(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número a redondear.|  

## Descripción

Esta función aproxima un número real al entero que se encuentre más cerca de él, por ejemplo, redondear 3.14 devolverá 3, mientras que redondear 5.59 devolverá 6. En el caso de que el número a redondear sea un medio entero (como 1.5, 3.5, 4.5, -3.5, etc.), éste se aproximará el entero **par** más cercano. Por ejemplo, redondear 2.5 devolverá 2, pero redondear 3.5 devolverá 4.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = round(3.37); //Devuelve 3  
b = round(1.66); //Devuelve 2  
c = round(17); //Devuelve 17  
d = round(12.5); //Devuelve 12  
e = round(7.5); //Devuelve 8  
```