# draw_background_tiled

Dibuja un background repetidamente.

## Sintaxis

  
```gml  
draw_background_tiled(back, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El indice del background a dibujar.|  
x|La coordenada en x desde donde se dibujará el background.|  
y|La coordenada en y desde donde se dibujará el background.|  

## Descripción

Esta función es muy similar a `draw_background()`, con la diferencia de que el background se dibuja repetidamente desde las coordenadas dadas hasta llenar la vista actual, o la sala, en caso de que no hayan vistas activas.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_background_tiled(bck_Sky, x, y);  
```