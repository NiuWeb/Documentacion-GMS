# ds_list_clear

Limpia todos los datos de la lista dada.

## Sintaxis

  
```gml  
ds_list_clear(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a limpiar.|  

## Descripción

Con esta función puede limpiar todos os datos de la lista dada. Esto **NO** destruye la estructura de datos (para ello debe usar `ds_list_destroy()`) solamente limpiara toda la información y regresa una lista vacía.

## Devuelve

Nada

## Ejemplo

  
```gml  
if count == 15 && !ds_list_empty(command_list){  
     ds_list_clear(command_list);  
     alarm[0] = room_speed;  
     ai_count = 0;  
}  
```  
El código anterior comprueba si una variable a alcanzado un valor específico, y si lo tiene limpia la ds_list indexada en la variable "command_list" establece una alarma y restablece otra variable a 0.