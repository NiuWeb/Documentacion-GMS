# draw_sprite_tiled

Dibuja un sprite y lo repite hasta rellenar la vista.

## Síntaxis

  
```gml  
draw_sprite_tiled(sprite, subimg, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sprite|El índice del sprite a dibujar.|  
subimg|El número de la subimagen del sprite a dibujar (0 es la primera).|  
x|La posición horizontal donde dibujar el sprite.|  
y|La posición vertical donde dibujar el sprite.|  

## Descripción

Esta función toma un sprite y lo dibuja repetidamente hasta que cruza el borde de la vista (o de la sala si no hay ninguna vista definida), iniciando desde las coordenadas dadas.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_sprite_tiled(sprite_index, image_index, x, y);  
```  
Se dibujará repetidamente el sprite actual de la instancia, hasta llenar la vista de la sala.