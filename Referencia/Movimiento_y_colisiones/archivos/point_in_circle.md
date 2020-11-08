# point_in_circle

Comprueba si el punto dado se encuentra dentro del área circular establecida.

## Sintaxis

  
```gml  
point_in_circle(px, py, x, y, r);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
px|La posición horizontal del punto a comprobar.|  
py|La posición vertical del punto a comprobar.|  
x|La posición horizontal del centro del área circular a comprobar.|  
y|La posición vertical del centro del área circular a comprobar.|  
r|El radio del área circular a comprobar.|  

## Descripción

Esta función permite definir un área circular y comprobar si el punto dado se encuentra en su interior (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
if(mouse_check_button_pressed(mb_left)) {  
    if(point_in_rectangle(mouse_x, mouse_y, room_width/2, room_height/2, 64))  
        room_goto(rmPlay);  
}  
```  
Al momento de presionar el botón izquierdo del ratón, se comprobará si el cursor se encuentra dentro del área circular posicionada en el centro de la sala actual y con un radio de 64px, y de ser así, se redirigirá a la sala rmPlay.