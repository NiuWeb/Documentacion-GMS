# dtan

devuelve la _tangente_ del ángulo dado (en grados).

## Síntaxis

  
```gml  
tan(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El ángulo al cual obtener la _tangente_.|  

## Descripción

Esta función permite obtener el valor del _tangente_ de un ángulo determinado.   
  
**NOTA:** Si val tiene un valor de 90 ± 180_n_ (siendo _n_ un número entero), la función ocasionará un error, pues la tangente de estos ángulos es infinito.

## Devuelve

Número real.

## Ejemplo

  
```gml  
A = tan(45); //devuelve 1  
```