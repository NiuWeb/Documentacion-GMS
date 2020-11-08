# arcsin

Devuelve el seno inverso de un número.

## Sintaxis

  
```gml  
arcsin(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El ángulo (en radianes) al cual obtener el seno inverso.|  

## Descripción

Esta función devuelve el seno inverso del número dado. Básicamente, si `sin(a) = b`, entonces `arcsin(b) = a`. El número resultante estará entre -π/2 y π/2.  
  
**NOTA:** Esta función sólo acepta números entre -1 y 1. Cualquier número fuera de este rango ocacionará un error.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = arcsin(0); //Devuelve 0  
```