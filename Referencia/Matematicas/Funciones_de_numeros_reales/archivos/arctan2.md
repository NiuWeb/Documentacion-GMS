# arctan2

Devuelve la tangente inversa (el ángulo) de un vector dado por determinados componentes.

## Síntaxis

  
```gml  
arctan2(b, a)  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
b|El componente vertical (cateto opuesto) del ángulo.|  
a|El componente horizontal (cateto adyacente) del ángulo.|  

## Descripción

Esta función obtiene la tangente inversa del ángulo que corresponde a un triángulo cuyo cateto opuesto es b y el adyacente es a. A diferencia de `arctan(n)`, esta función no corre el riesgo de una división por cero.   
  
**NOTA:** El valor es devuelto en radianes, no en grados.

## Devuelve

Número real

## Ejemplo

  
```gml  
var a = arctan2(1, 1); //devuelve π/4 = 0.79 apróx.  
```  
Dentro de un triángulo rectángulo, un ángulo cuyo cateto opuesto y adyacente sean 1 es π/4 _rad_.