# ystart

La posición vertical inicial de una instancia.

## Sintaxis

  
```gml  
ystart;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable almacena la posición vertical inicial en la que la instancia fue creada. El valor de esta variable puede ser modificado a gusto (esto no afectará la posición actual de la instancia).

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(salud <= 0) {  
    x = xstart;  
    y = ystart;  
    vidas--;  
}  
```  
En caso de que la variable `salud` sea menor o igual a 0, la instancia volverá a su posición inicial y se restará 1 a la variable `vidas`.