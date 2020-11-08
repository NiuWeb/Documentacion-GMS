# irandom_range

Devuelve un número entero aleatorio entre dos límites de un rango.

## Sintaxis

  
```gml  
irandom_range(n1, n2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
n1|El límite inferior del rango en el cual se generará el número.|  
n2|El límite superior del rango en el cual se generará el número.|  

## Descripción

Esta función devuelve un número entero aleatorio dentro del rango especificado por los argumentos dados. El límite superior (`n2`) **puede** ser generado.  
  
**NOTA:** Esta función generará los mismos resultados (en el mismo orden) cada vez que se ejecuta el juego. Esto gracias a que Game Maker Studio genera la misma semilla aleatoria inicial. Para evitar esto, usar `randomize()` al inicio del juego para generar una nueva semilla aleatoria.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = irandom_range(3, 9); //Devuelve un número entero aleatorio entre 3 y 9. Tanto 6 como 9 pueden generarse.  
b = irandom_range(-5, 6); //Devuelve un número entero aleatorio entre  -5 y 6. Tanto -5 como 6 pueden generarse.  
c = irandom_range(2.8, 7.47); //Devuelve un número entero aleatorio entre 2 y 7, ya que los límites del rango son aproximados al menor entero más cercano.  
```