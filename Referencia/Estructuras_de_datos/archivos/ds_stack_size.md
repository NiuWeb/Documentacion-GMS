# ds_stack_size

Regresa el número de valores guardados en la pila dada.

## Síntaxis

  
```gml  
ds_stack_size(ds);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la estructura de datos a comprobar.|  

## Descripción

Esta función regresa el "tamaño" de la pila. Es decir, el número de elementos guardados en ésta.

## Devuelve

Número real

## Ejemplo

  
```gml  
if !ds_stack_empty(control_stack){  
     num = ds_stack_size(control_stack);  
}  
```  
El código anterior comprueba si la pila no esta vacía. Si no lo está, obtiene el número de elementos que contiene y guarda ese valor dentro de una variable.