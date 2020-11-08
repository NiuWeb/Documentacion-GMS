# draw_set_colour

Obtiene el color base actual para las funciones de dibujo.

## Sintaxis

  
```gml  
draw_get_colour();  
```  

## Argumentos

Ninguno.

## Descripción

Esta función permite obtener el color de dibujo actual, definido por la función `draw_set_colour()`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(draw_get_colour() <> c_blue)  
{  
draw_set_colour(c_blue);  
}  
```  
El código anterior comprueba si el color de dibujo actual es `c_blue`. Si no lo es, lo establece a dicho valor.