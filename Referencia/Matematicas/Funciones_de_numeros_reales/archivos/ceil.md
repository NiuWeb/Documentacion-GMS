# ceil

Aproxima un número real al mayor entero más cercano.

## Sintaxis

  
```gml  
ceil(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número a aproximar.|  

## Descripción

Esta función aproxima un número real al mayor entero más cercano. Por ejemplo, aproximar 3.14 al mayor entero más cercano devolverá 4, lo mismo con 3.99, 3.1 ó 3.5.

## Devuelve

Número entero

## Ejemplo

  
```gml  
a = ceil(5.1); //Devuelve 6  
b = ceil(3.33); //Devuelve 4  
c = ceil(8.991); //Devuelve 8  
d = ceil(13); //Devuelve 13  
e = ceil(0); //Devuelve 0  
```