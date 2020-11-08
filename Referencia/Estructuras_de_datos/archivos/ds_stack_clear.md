# ds_stack_clear

Elimina la información que contiene la pila dada.

## Síntaxis

  
```gml  
ds_stack_clear(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la estructura de datos a limpiar.|  

## Descripción

Puede usar esta función para remover toda la información contenida en la pila que ha sido indicada. Esto **NO** elimina la estructura de datos (para eliminarla es necesario usar `ds_stack_destroy()`) solamente remueve toda la información y regresa una pila vacía.

## Devuelve

Nada

## Ejemplo

  
```gml  
if ai_count = 15 && !ds_stack_empty(AI_stack) {  
     ds_stack_clear(AI_stack);  
     alarm[0] = room_speed;  
     ai_count = 0;  
}  
```  
El código anterior comprueba si la variable indicada tiene el valor especificado. Al cumplirse, la pila (ds_stack) indexada en la variable "AI_stack" es limpiada, establece una alarma y regresa la variable a 0.