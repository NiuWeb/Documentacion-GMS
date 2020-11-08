# ds_stack_push

Añade el valor (o valores dados) arriba de la pila.

## Síntaxis

  
```gml  
ds_stack_push(ds, val [, val2, ... val15]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la pila de la que se tomará.|  
val|El valor a añadir en la pila.|  
[val2, ..., val13]|Valores opcionales a añadir a la pila.|  

## Descripción

Esta función permite _apilar_ (añadir) un valor, el cual puede ser un número real o una cadena de texto a la pila indicada. Esta función puede tomar hasta 14 argumentos opcionales, permitiendo apilar múltiples valores al mismo tiempo en una pila.

## Devuelve

Nada

## Ejemplo

  
```gml  
move_stack = ds_stack_create();  
ds_stack_push(move_stack, x, y, x, y + 200, x + 200, y + 200, x +200, y);  
```  
El código anterior crea una nueva pila(ds_stack) y almacena su indice en la variable "move_stack". Entonces añade valores a la pila, que serán usados en un futuro.