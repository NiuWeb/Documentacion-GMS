# room_first

El índice de la primera _room_ en el juego.

## Sintaxis

  
```gml  
room_first;  
```  

## Descripción

Esta variable de **sólo lectura** devuelve el índice de la primera _room_ del juego (definida por el orden en que las _rooms_ aparecen en el árbol de recursos y **no** por el orden en que se crearon).

## Devuelve

Número real

## Ejemplo

  
```gml  
if vidas < 1  
{  
    room_goto(room_first);  
}  
```  
El código anterior comprobará la variable "vidas" y si es menor de 1 nos llevará a la primera _room_ del juego.