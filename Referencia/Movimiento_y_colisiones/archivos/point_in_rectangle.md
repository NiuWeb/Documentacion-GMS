# point_in_rectangle

Comprueba si el punto dado se encuentra dentro del área rectangular establecida.

## Sintaxis

  
```gml  
point_in_rectangle(px, py, x1, y1, x2, y2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
px|La posición horizontal del punto a comprobar.|  
py|La posición vertical del punto a comprobar.|  
x1|La posición horizontal del primer punto del área rectangular.|  
y1|La posición vertical del primer punto del área rectangular.|  
x2|La posición horizontal del segundo punto del área rectangular.|  
y2|La posición vertical del segundo punto del área rectangular.|  

## Descripción

Esta función permite definir un área rectangular y comprobar si el punto dado se encuentra dentro de ésta (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
if(point_in_rectangle(mouse_x, mouse_y, 32, 32, 96, 64))  
    show_message("¡El cursor está dentro del recuadro!");  
```  
En el ejemplo anterior, se comprueba si el cursor se encuentra dentro de un área rectangular dada, y de ser así, mostrará un mensaje indicándolo.