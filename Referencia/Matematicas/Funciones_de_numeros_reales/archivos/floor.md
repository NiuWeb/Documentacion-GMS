# floor

Aproxima un número real al menor entero más cercano.

## Sintaxis

  
```gml  
floor(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número a aproximar.|  

## Descripción

Básicamente, esta función elimina las cifras decimales de un número real. Por ejemplo, aproximar 3.77 hacia su menor entero dará como resultado 3. Lo mismo con 3.01 o 3.999

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = floor(13.15); //Devuelve 13  
b = floor(20); //Devuelve 20  
c = floor(8.79); //Devuelve 8  
d = floor(-17.99); //Devuelve -17  
```