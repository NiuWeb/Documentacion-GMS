# lerp

Devuelve la interpolación lineal de dos valores con la cantidad dada.

## Sintaxis

  
```gml  
lerp(a, b, c);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
a|El primer valor a interpolar.|  
b|El segundo valor a interpolar.|  
c|La cantidad a interpolar.|  

## Descripción

Con esta función se puede obtener el valor que se encuentra una posición entre otros valores según el porcentaje dado. Por ejemplo, `lerp(0, 16, 0.5)` devolverá 8, porque 8 es el 50% entre 0 y 16.  
La fórmula de la interpolación lineal es `a + (b-a)*c`

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = lerp(10, 15, 0.5); //Devuelve 12.5  
c = lerp(12, 18, 1.5); //Devuelve 21.  
d = lerp(21, 3, 0.5); //Devuelve 12.  
```