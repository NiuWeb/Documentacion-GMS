# draw_background_part

Dibuja una parte de un _background_ en la posición dada.

## Síntaxis

  
```gml  
draw_background_part(back, left, top, width, height, x, y);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
back|El índice del _background_ a dibujar. (Número real o constante de nombre).|  
left| La coordenada horizontal de la ezquina superior izquierda desde donde dibujar el _background_ |  
top| La coordenada vertical de la ezquina superior izquierda desde donde dibujar el _background_ |  
width| El anchor del área del background a dibujar. |  
height| La altura del área del background a dibujar. |  

## Descripción

Esta función permite dibujar una parte de cualquier background en la posición dada dentro de la habitación. Trabaja de forma similar a `draw_background()`, con la diferencia de que es necesario especificar las coordenadas relativas(**dentro** del _background_) para definir el área del mismo que se dibujará. Esto significa que definir los parámetros `left` y `top` a 0 dibujará el background desde la ezquina superior izquierda, y este punto será el origen desde donde se tomarán las coordenadas de dibujo.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_background_part(bck_Sky, 8, 8, 32, 32, x, y);  
```  
Se dibuja un área del background `bck_Sky` de 32x32 empezando con un margen de 8px desde arriba y la izquierda, en las coordenadas actuales.