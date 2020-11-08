# effect_clear

Limpia todos los efectos creados con el sistema de partículas predefinido.

## Sintaxis

  
```gml  
effect_clear();  
```  

## Descripción

Elimina todas las partículas que fueron creadas con las funciones `effect_create_above` o `effect_create_below`.

## Devuelve

Nada

## Ejemplo

  
```gml  
effect_clear();  
room_goto_next();  
          
```  
En el ejemplo se eliminan las partículas para que no aparezcan en la siguiente room.