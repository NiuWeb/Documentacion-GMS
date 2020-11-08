# ds_list_destroy

Destruye la lista dada y la remueve de la memoria.

## Sintaxis

  
```gml  
ds_list_destroy(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a destruir.|  

## Descripción

Esta función eliminará la estructura de datos (la lista dada) de la memoria, liberando el espacio que estaba ocupando además de eliminar todos los valores que contenía.. Esta función siempre debe de ser usada cuando se deje de utilizar la lista para evitar fugas de memoria que podrían ralentizar bloquear su juego.

## Devuelve

Nada

## Ejemplo

  
```gml  
if lives == 0{  
     ds_list_destroy(AI_list);  
     room_goto(rm_Menu);  
}  
```  
El código anterior comprueba el valor de la variable global "lives", si es 0, destruye la lista indexada en la variable "AI_list" y luego cambia de room.