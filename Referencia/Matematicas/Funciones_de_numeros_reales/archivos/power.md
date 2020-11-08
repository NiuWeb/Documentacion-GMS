# power

Devuelve un valor multiplicado por sí mismo un número dado de veces.

## Sintaxis

  
```gml  
power(a, n);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
a|El valor a multiplicar por sí mismo.|  
n|La cantidad de veces a multiplicar por sí mismo el número.|  

## Descripción

Esta función devuelve un número multiplicado por sí mismo `n` veces (`an`).  
  
**NOTA:** A diferencia de la función `sqrt()`, obtener la raíz par de un número negativo con esta función (_ej:_ `power(-1, 0.5)`) no producirá un error, sino que devolverá `NaN`, un valor especial que en _GameMaker: Studio_ es considerado como número real por la función `is_real()`.

## Devuelve

Número real

## Ejemplo

  
```gml  
a = power(2, 3); //Devuelve 8, porque 2*2*2=8  
b = power(3, 3); //Devuelve 27, porque 3*3*3=27  
c = power(5, -1); //Devuelve 0.2, porque 1/5=0.2  
```