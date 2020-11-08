# draw_background_stretched

Dibuja un background redimensionado.

## Síntaxis

  
```gml  
draw_background_stretched(back, x, y, w, h);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El índice del background a dibujar, puede ser una constante o un número real.|  
x|La posición horizontal desde donde dibujar el background.|  
y|La posición vertical desde donde dibujar el background.|  
w|El anchor (en pixeles) del background.|  
h|La altura (en pixeles) del background.|  

## Descripción

Esta función es muy similar a `draw_background()`, con la diferencia de que permite modificar su anchor y altura.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_background_stretched(bck_Sky, 10, 10, 100, 100);  
```