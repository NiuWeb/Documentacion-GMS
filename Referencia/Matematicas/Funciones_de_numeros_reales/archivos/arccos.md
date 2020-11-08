# arccos

Devuelve el coseno inverso de un número.

## Sintaxis

  
```gml  
arccos(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El ángulo (en radianes) al cual obtener el coseno inverso|  

## Descripción

Esta función devuelve el coseno inverso de el valor dado. Básicamente, si `cos(a) = b`, entonces `arccos(b) = a`. El número resultante estará entre π y 0.  
**NOTA:** Esta función sólo acepta como argumento un número entre -1 y 1. Cualquier número fuera de este rango ocacionará un error.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = arccos(0); //Devuelve pi/2  
```