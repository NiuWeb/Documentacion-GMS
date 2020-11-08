# draw_background_stretched_ext

Dibuja un background redimensionado con color y opacidad personalizados.

## Síntaxis

  
```gml  
draw_background_stretched_ext(back, x, y, w, h, colour, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El índice del background a dibujar, puede ser una constante o un número real.|  
x|La posición horizontal desde donde dibujar el background.|  
y|La posición vertical desde donde dibujar el background.|  
w|El anchor (en pixeles) del background.|  
h|La altura (en pixeles) del background.|  
colour| El color con el cual mezclar el _background_ (usar `c_white` para dibujarlo normalmente). |  
alpha|La opacidad del _background_ (1 es totalmente opaco).|  

## Descripción

Esta función es una mezcla entre `draw_background_stretched()` y `draw_background_ext()`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_background_stretched_ext(bck_Sky, x, y, 200, 200, c_white, 0.5);  
```