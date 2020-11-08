# game_load_buffer

Carga un juego guardado desde un búfer.

## Sintaxis

  
```gml  
game_load_buffer(buffer);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
buffer|La identificación del búfer del cual cargar el juego.|  

## Descripción

Esta función permite cargar un estado del juego. El juego es cargado de un búfer de tipo _grow_ previamente creado, el cual tiene dentro de sí el estado del juego guardado utilizando la función `game_save_buffer()`.

## Devuelve

Nada

## Ejemplo

  
```gml  
if(keyboard_check(ord("L")))  
    game_load_buffer(gamesave[3]);  
```  
Si se presiona la tecla **L**, se cargará el estado del juego desde el búfer encontrado en el índice 3 de la variable `gamesave`.