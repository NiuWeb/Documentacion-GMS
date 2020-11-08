# ds_stack_destroy

Elimina la pila dada y libera la memoria usada.

## Síntaxis

  
```gml  
ds_stack_destroy(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la estructura de datos a eliminar.|  

## Descripción

Esta función permite remover la pila de la memoria, liberando los recursos usados y eliminando todos los valores que contiene. Esta función debe ser usada cuando se ha terminado de utilizar la pila para prevenir fugas de memoria que reduzcan el rendimiento del juego o provoquen fallos.

## Devuelve

Nada

## Ejemplo

  
```gml  
if lives = 0{  
     ds_stack_destroy(AI_stack);  
     room_goto(rm_Menu);  
}  
```  
El código anterior comprueba el valor de la variable global reservada "lives" y si ésta es 0, elimina la pila (ds_stack) indexada en la variable "AI_stack" y luego cambia de habitación.