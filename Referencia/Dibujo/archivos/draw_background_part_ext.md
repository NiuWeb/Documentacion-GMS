# draw_background_part_ext

Dibuja una parte de un _background_ con escala, color y opacidad personalizadas.

## Síntaxis

  
```gml  
draw_background_part_ext(back, left, top, width, height, x, y, xscale, yscale, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El índice del _background_ a dibujar. (Número real o constante de nombre).|  
left| La coordenada horizontal de la ezquina superior izquierda desde donde dibujar el _background_ |  
top| La coordenada vertical de la ezquina superior izquierda desde donde dibujar el _background_ |  
width| El anchor del área del background a dibujar. |  
height| La altura del área del background a dibujar. |  
xscale|La escala horizontal del _background_ (1 es tamaño original).|  
yscale|La escala vertical del _background_ (1 es tamaño original).|  
colour| El color con el cual mezclar el _background_ (usar `c_white` para dibujarlo normalmente). |  
alpha|La opacidad del _background_ (1 es totalmente opaco).|  

## Descripción

Esta función es una mezcla entre `draw_background_part()` y `draw_background_ext()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_background_part_ext(bck_Sky, 8, 8, 32, 32, x, y, 2, 0.5, c_black, 1);  
```