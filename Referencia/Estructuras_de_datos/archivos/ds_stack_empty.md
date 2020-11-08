# ds_stack_empty

Comprueba si la pila dada esta vacía o no.

## Síntaxis

  
```gml  
ds_stack_empty(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la estructura de datos a comprobar.|  

## Descripción

Con esta función puede comprobar si la pila dada esta vacía (regresa `true`) o no (regresa `false`).

## Devuelve

Boleano

## Ejemplo

  
```gml  
if ai_count = 15 && !ds_stack_empty(AI_stack) {  
     ds_stack_clear(AI_stack);  
     alarm[0] = room_speed;  
     ai_count = 0;  
}  
```  
El código anterior comprueba si las variables indicadas tienen los valor especificados. Al cumplirse, la pila (ds_stack) indexada en la variable "AI_stack" es limpiada, establece una alarma y regresa las variables a 0.