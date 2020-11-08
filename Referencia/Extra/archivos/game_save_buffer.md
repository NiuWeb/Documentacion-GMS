# game_save_buffer

Guarda el juego en un búfer.

## Sintaxis

  
```gml  
game_save_buffer(buffer);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
buffer|El identificador del búfer en donde guardar el juego.|  

## Descripción

Esta función permite guardar el estado actual del juego en un búfer de tipo _grow_ creado previamente.  
  
**NOTA:** Esta función es muy limitada y está diseñada para ofrecer un sistema de guardado fácil para los principiantes. Probablemente, un usuario más avanzado prefiera programar su propio sistema de guardado utilizando otras funciones de archivos. Cabe mencionar que esta función no guarda ningún recurso dinámico como estructuras de datos, superficies ni _backgrounds_ o _sprites_ cargados externamente.

## Devuelve

Nada

## Ejemplo

  
```gml  
partida = buffer_create(32, buffer_grow, 1);  
game_save_buffer(partida);  
```  
Se guarda el estado del juego en el búfer `partida`.