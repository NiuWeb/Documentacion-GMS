# logn

Obtiene el logaritmo en base _n_ del número dado.

## Síntaxis

  
```gml  
logn(n, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
n|La base del logaritmo|  
val|El número real a quien obtener el logaritmo en base n.|  

## Descripción

En resumen, esta función obtiene la cantidad de veces que el número n debe multiplicarse por sí mismo para obtener el número val

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = logn(5, 25); //devuelve 2, pues 52 = 25  
b = logn(3, 729); //Devuelve 6, pues 36 = 729  
```