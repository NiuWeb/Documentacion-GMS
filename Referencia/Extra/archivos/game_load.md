# game_load

Carga un juego guardado desde un archivo.

## Sintaxis

  
```gml  
game_load(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo a cargar.|  

## Descripción

Esta función permite cargar un juego previamente guardado (utilizando `game_save()`).

## Devuelve

Nada

## Ejemplo

  
```gml  
if(keyboard_check(ord("L")))  
    game_load("Checkpoints/savegame3.sav");  
```  
Si se presiona la tecla **L**, se cargará el juego del archivo `"savegame3.sav"` encontrado en el directorio `"Checkpoints"`.