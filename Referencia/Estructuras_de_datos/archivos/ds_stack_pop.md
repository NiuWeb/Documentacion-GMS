# ds_stack_pop

Toma el valor que se encuentra arriba de la Pila.

## Síntaxis

  
```gml  
ds_stack_pop(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la Pila de la que se tomará.|  

## Descripción

Esta función permite _tomar_ el primer valor de la pila, removiéndolo de ésta y regresando dicho valor para ser almacenado en una variable.

## Devuelve

Número real o cadena de texto.

## Ejemplo

  
```gml  
if !ds_stack_empty(move_stack){  
     var xx, yy;  
     xx = ds_stack_pop(move_stack);  
     yy = ds_stack_pop(move_stack);  
     move_towards_point(xx, yy, 4);  
}  
```  
El código anterior comprueba si la pila indexada en la variable "move_stack" no esta vacía. Si no lo está, entonces toma dos valores de la pila y los usa para establecer su dirección de movimiento.