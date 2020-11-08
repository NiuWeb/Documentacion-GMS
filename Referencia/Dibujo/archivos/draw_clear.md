# draw_clear

Limpia la superficie de dibujo actual con el color dado.

## Sintaxis

  
```gml  
draw_clear(col);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
col|El color con el cual limpiar la pantalla.|  

## Descripción

Esta función permite limpiar la superficie de dibujo actual con el color dado (sin opciones de opacidad). Sólo debe ser utilizada dentro del evento _Draw_ de alguna instancia, o bien para limpiar superficies cuando se necesita dibujar nuevamente en ellas.

## Devuelve

Nada

## Ejemplo

  
```gml  
    
///Evento Draw  
draw_clear(c_black)  
```  
El código anterior limpia la pantalla con el color negro.