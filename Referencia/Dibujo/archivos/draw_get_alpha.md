# draw_set_alpha

Obtiene la opacidad base actual para las funciones de dibujo.

## Sintaxis

  
```gml  
draw_get_alpha();  
```  

## Argumentos

Ninguno.

## Descripción

Esta función permite obtener el valor actual de la opacidad de dibujo, establecida por la función `draw_set_alpha()`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(draw_get_alpha() <> 1) //Si la opacidad actual es diferente de 1  
{  
draw_set_alpha(1); //Establecerla a 1.  
}  
```  
El código anterior comprueba si la opacidad de dibujo actual es 1. Si no lo es, la establece a dicho valor.