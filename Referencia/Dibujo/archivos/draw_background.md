# draw_background

Dibuja un background sin colorearlo y sin transparencia.

## Sintaxis

  
```gml  
draw_background(back, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El indice del background a dibujar.|  
x|La coordenada en x desde donde se dibujará el background.|  
y|La coordenada en y desde donde se dibujará el background.|  

## Descripción

Con esta función se puede dibujar cualquiera de los backgrounds activos del room actual en la posición deseada, el background siempre empezará desde la esquina superior izquierda, sobre la posición (x, y) especificada.

## Devuelve

Nada

## Ejemplo

  
```gml  
draw_background(bck_Sky, view_xview[0], view_yview[0]);  
```  
El código anterior, dibuja el background indexado en `bck_Sky` en la posición de la view[0].