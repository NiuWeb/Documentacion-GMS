# draw_background_ext

Dibuja un _background_ con color, opacidad, escala y ángulo personalizados.

## Síntaxis

  
```gml  
draw_background_ext(back, x, y, xscale, yscale, rot, colour, alpha);  
    
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El índice del _background_ a dibujar. (Número real o constante de nombre).|  
x|La posición horizontal donde dibujar el _background_.|  
y|La posición vertical donde dibujar el _background_.|  
xscale|La escala horizontal del _background_ (1 es tamaño original).|  
yscale|La escala vertical del _background_ (1 es tamaño original).|  
rot|La rotación del _background_ (en grados).|  
colour| El color con el cual mezclar el _background_ (usar `c_white` para dibujarlo normalmente). |  
alpha|La opacidad del _background_ (1 es totalmente opaco).|  

## Descripción

Esta función permite dibujar un _backrground_ determinado de forma similar a `draw_background()`, con la diferencia de que es posible establecer propiedades como la escala, rotación, color y opacidad del mismo.  
  
**NOTA:** La mezcla de colores es recomendada en la plataforma HTML5 **sólo** cuando el _WebGL_ está activo. Anque esta mezcla pueda realizarse aun sin _WebGL_, esto provocará que se cree una copia del _background_ (u otro recurso, como _sprites_) con las modificaciones de color hechas, almacenándoce en la caché. Esto es muy poco óptimo, y muchos cambios de mezcla de color ralentizará el rendimiento del juego. Si aún así usted no desea usar _WebGL_ y necesita realizar mezclas de color, puede considerar limitar el tamaño del caché de los sprites (y backgrounds) usando la función `sprite_set_cache_size()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_background_ext(bck_Sky, 0, 0, background_xscale[0], background_yscale[0], 0, c_red, 0.5);  
    
```  
Se dibuja el background _bck_Sky_ en la posición (0, 0) de la sala, con la escala actual del background de la sala. El _background_ no está rotado (0°), se mezclará de color rojo y tendrá una opacidad del 50%.