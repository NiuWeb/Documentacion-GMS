# rectangle_in_rectangle

Comprueba si un área rectangular colisiona con otra.

## Sintaxis

  
```gml  
rectangle_in_rectangle(sx1, sy1, sx2, sy2, dx1, dy1, dx2, dy2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
sx1|El componente horizontal del primer punto del área rectangular fuente.|  
sy1|El componente vertical del primer punto del área rectangular fuente.|  
sx2|El componente horizontal del segundo punto del área rectangular fuente.|  
sy2|El componente vertical del segundo punto del área rectangular fuente.|  
dx1|El componente horizontal del primer punto del área rectangular de destino.|  
dy1|El componente vertical del primer punto del área rectangular de destino.|  
dx2|El componente horizontal del segundo punto del área rectangular de destino.|  
dy2|El componente vertical del segundo punto del área rectangular de destino.|  

## Descripción

Esta función permite comprobar si el área rectangular fuente definida colisiona, completa o parcialmente, con el área rectangular de destino definida. Si las áreas rectangulares no colisionan, la función devolverá 0. Si el área rectangular fuente se encuentra completamente dentro del área de destino, la función devolverá 1, y si el área fuente colisiona parcialmente con el área de destino, la función devolverá 2.

## Devuelve

Número real.