# angle_difference

Devuelve la diferencia entre dos ángulos

## Sintaxis

  
```gml  
angle_difference(a, b);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
a|El primer ángulo a evaluar|  
b|El segundo ángulo a evaluar|  

## Descripción

Esta función devuelve la menor diferencia entre dos ángulos, como un valor entre -180 grados y 180 grados.  
  
**NOTA:** Un ángulo positivo es en sentido anti-horario, mientras que uno negativo es en sentido horario.

## Devuelve

Nùmero real

## Ejemplo

  
```gml  
var pd = point_direction(x, y, mouse_x, mouse_y);  
var dd = angle_difference(image_angle, pd);  
image_angle += min(abs(dd), 10) * sign(dd);  
```  
Se obtiene la diferencia de ángulos entre la rotaciòn del _sprite_ actual y el àngulo que se forma con la posición actual del cursor, con el fin de realizar un giro suavizado hacia èste.