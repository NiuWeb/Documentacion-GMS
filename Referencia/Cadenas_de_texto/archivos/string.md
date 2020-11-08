# string

Convierte un número real a una cadena de texto.

## Sintaxis

  
```gml  
string(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número real a convertir|  

## Descripción

Esta función permite convertir un número real a una cadena de texto. Si el número es entero, se convertirá sin cifras decimales. De lo contrario, se convertirá con dos cifras decimales.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
a = 25;  
b = string(a);  
c = "El número " + b + " es el que le sigue al número " + string(a - 1); //Devuelve "El número 25 es el que le sigue al número 24  
```  
Se convierten los valores necesarios a cadena de texto, para poderlos concatenar y formar el mensaje deseado.