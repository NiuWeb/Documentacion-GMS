# radtodeg

Convierte un valor en radianes a grados.

## Sintaxis

  
```gml  
radtodeg(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número en radianes a convertir a grados.|  

## Descripción

Esta función permite convertir un número real expresado en radianes a grados, usando la fórmula `(180/pi)*val`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = radtodeg(pi); //Devuelve 180  
b = radtodeg(pi/4); //Devuelve 45.  
```