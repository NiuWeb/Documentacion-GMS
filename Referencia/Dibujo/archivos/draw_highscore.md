# draw_highscore

Dibuja la table de _highscores_ en la sala dentro del rectángulo dado, utilizando la fuente, alfa y color establecidos actualmente.

## Síntaxis

  
```gml  
draw_highscore( x1, y1, x2, y2 );  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|El componente horizontal del primer punto del rectángulo.|  
y1|El componente vertical del primer punto del rectángulo.|  
x2|El componente horizontal del segundo punto del rectángulo.|  
y2|El componente vertical del segundo punto del rectángulo.|  

## Descripción

Esta simple función permite dibujar la lista local de puntajes altos actual utilizando las configuraciones de dibujo (fuente, color y opacidad) actuales, dentro del rectángulo específico.

## Devuelve

Nada.

## Ejemplo

  
```gml  
draw_highscore(100, 100, room_width - 100, room_height - 100);  
```