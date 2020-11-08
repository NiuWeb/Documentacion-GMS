# tan

devuelve la _tangente_ del ángulo dado (en radianes).

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
  
**NOTA:** Si val tiene un valor de π/2 ± _n_π (siendo _n_ un número entero), la función ocasionará un error, pues la tangente de estos ángulos es infinito.

## Devuelve

Número real.

## Ejemplo

  
```gml  
A = tan(pi/4); //devuelve 1  
```