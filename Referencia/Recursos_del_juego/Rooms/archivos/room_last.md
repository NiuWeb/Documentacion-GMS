# room_last

El índice de la última _room_ en el juego.

## Sintaxis

  
```gml  
room_last;  
```  

## Descripción

Esta variable de **sólo lectura** devuelve el índice de la última _room_ del juego (definida por el orden en que las _rooms_ aparecen en el árbol de recursos y **no** por el orden en que se crearon.

## Devuelve

Número real

## Ejemplo

  
```gml  
if keyboard_check_pressed(ord("Q"))  
{  
    room_goto(room_last);  
}  
```  
El código anterior comprueba si se ha pulsado la tecla "Q" y, de ser así, se pasa a la última _room_ del juego.