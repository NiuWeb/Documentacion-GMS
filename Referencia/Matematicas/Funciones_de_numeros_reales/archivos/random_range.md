# random_range

Devuelve un número real aleatorio entre dos límites de un rango.

## Sintaxis

  
```gml  
random_range(n1, n2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
n1|El límite inferior del rango en el cual se generará el número.|  
n2|El límite superior del rango en el cual se generará el número.|  

## Descripción

Esta función devuelve un número real aleatorio dentro del rango especificado por los dos valores argumentados. El límite superior nunca será generado.  
  
**NOTA:** Esta función generará los mismos resultados (en el mismo orden) cada vez que se ejecuta el juego. Esto gracias a que Game Maker Studio genera la misma semilla aleatoria inicial. Para evitar esto, usar `randomize()` al inicio del juego para generar una nueva semilla aleatoria.  

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = random_range(3, 9); //Devuelve un número real aleatorio entre 0 y 9.  
```