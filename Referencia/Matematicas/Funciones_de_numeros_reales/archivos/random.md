# random

Devuelve un número real aleatorio entre 0 y el número argumentado.

## Sintaxis

  
```gml  
random(n);  
```  

## Argumentos

Ninguno

## Descripción

Esta función devuelve un número real (puede tener cifras decimales) entre 0 y `n`. El número argumentado nunca será generado.  
  
**NOTA:** Esta función generará los mismos resultados (en el mismo orden) cada vez que se ejecuta el juego. Esto gracias a que GameMaker: Studio genera la misma semilla aleatoria inicial. Para evitar esto, usar `randomize()` al inicio del juego para generar una nueva semilla aleatoria.

## Devuelve

Número real

## Ejemplo

  
```gml  
a = random(10); //Genera un número entre 0 y 9.  
b = random(3.8); //Genera un número entre 0 y 3.8. Podrá generarse 3.79, pero nunca 3.8  
```