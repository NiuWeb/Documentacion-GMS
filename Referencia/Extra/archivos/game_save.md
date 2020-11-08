# game_save

Guarda el juego en un archivo.

## Sintaxis

  
```gml  
game_save(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo en donde guardar (de no existir, se creará).|  

## Descripción

Esta función permite realizar un guardado básico del juego en un archivo determinado.  
  
**NOTA:** Esta función es muy limitada y está diseñada para ofrecer un sistema de guardado fácil para los principiantes. Probablemente, un usuario más avanzado prefiera programar su propio sistema de guardado utilizando otras funciones de archivos. Cabe mencionar que esta función no guarda ningún recurso dinámico como estructuras de datos, superficies ni _backgrounds_ o _sprites_ cargados externamente.

## Devuelve

Nada.

## Ejemplo

  
```gml  
if(keyboard_check(ord("S")))  
    game_save("Checkpoints/savegame3.sav");  
```  
Si se presiona la tecla **S**, se guardará el juego en el archivo `"savegame3.sav"` dentro del directorio `"Checkpoints"`.