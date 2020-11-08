# draw_background_tiled_ext

Dibuja un background repetidamente con escala, color y opacidad personalizados.

## Sintaxis

  
```gml  
draw_background_tiled_ext(back, x, y, xscale, yscale, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El indice del background a dibujar.|  
x|La coordenada en x desde donde se dibujará el background.|  
y|La coordenada en y desde donde se dibujará el background.|  
xscale|La escala horizontal del _background_ (1 es tamaño original).|  
yscale|La escala vertical del _background_ (1 es tamaño original).|  
colour| El color con el cual mezclar el _background_ (usar `c_white` para dibujarlo normalmente). |  
alpha|La opacidad del _background_ (1 es totalmente opaco).|  

## Descripción

Esta función es una mezcla entre `draw_background_tiled()` y `draw_background_ext().`.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_background_tiled_ext(bck_Sky, x, y, 2, 2, c_red, 0.5);  
```