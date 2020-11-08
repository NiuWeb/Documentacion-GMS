# ds_list_empty

Devuelve si la lista dada esta vacía o no.

## Sintaxis

  
```gml  
ds_list_empty(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a comprobar.|  

## Descripción

Con esta función puede comprobar si la lista dada esta vacía (devuelve `true`) o no (devuelve `false`).

## Devuelve

Boleano

## Ejemplo

  
```gml  
if count == 15 && !ds_list_empty(command_list){  
      ds_list_clear(command_list);  
      alarm[0] = room_speed;  
      ai_count = 0;  
}  
```  
El código anterior comprueba si la variable "count" ha alcanzado un valor especifico y si la lista indexada en la variable "command_list" no esta vacía; de ser así limpiará la lista, establecerá una alarma y establecerá la variable "ai_count" a 0.