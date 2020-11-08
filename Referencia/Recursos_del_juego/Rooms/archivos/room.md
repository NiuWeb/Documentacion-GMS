# room

El índice de la _room_ actual.

## Sintaxis

  
```gml  
room;  
```  

## Descripción

Esta variable contiene el índice de la _room_ actual en la que el juego se encuentra. Esto **no** es una variable de sólo lectura, sin embargo cambiando esto no cambiará el valor del índice para la _room_ actual, sino que cambiará la _room_ para que coincida con el índice al que ha establecido la variable. Debe tener cuidado al hacer esto, ya que si el índice al que se cambia la variable no es válido el juego lanzará un error y se cerrará. En general, es mucho mejor usar `room_goto()` para cambiar de _room_.

## Devuelve

Número Real

## Ejemplo

  
```gml  
if room_next(room) != -1  
    {  
    room_goto(room_next(room));  
    }  
```  
El código anterior verificará si la _room_ siguiente existe y si es así, irá a ella.