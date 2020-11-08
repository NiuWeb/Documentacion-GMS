# ds_stack_top

Lee el valor que se encuentra arriba de la pila.

## Síntaxis

  
```gml  
ds_stack_top(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la pila a leer.|  

## Descripción

Esta función permite _solamente leer_ el primer valor de la pila (El que se encuentra _hasta arriba_). Esto no _remueve_ el valor, por lo que puede ser leído nuevamente en el futuro con esta función o por la función `ds_stack_pop()`.

## Devuelve

Número real o Cadena de texto

## Ejemplo

  
```gml  
num = ds_stack_top(control_stack);  
```  
El código anterior lee el valor de la pila indexada en la variable "control_stack" y lo almacena en la variable "num".