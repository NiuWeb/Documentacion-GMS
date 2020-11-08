# clamp

Mantiene un número real dentro del rango dado.

## Síntaxis

  
```gml  
clamp(val, minv, maxv);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El valor a restringir.|  
minv|El valor mínimo que podrá tener val.|  
maxv|El valor máximo que podrá tener val.|  

## Descripción

Esta función permite restringir un número real dentro de un rango de números determinado. Básicamente, si el número val es menor que minv, la función devolverá minv, y si val es mayor que maxv, la función devolverá maxv.

## Devuelve

Número real.

## Ejemplo

  
```gml  
clamp(5, 1, 10); //devuelve 5  
clamp(5, 6, 10); //devuelve 6  
clamp(-5, 1, 10); //devuelve 1  
clamp(7, 1, 4); //devuelve 4  
```