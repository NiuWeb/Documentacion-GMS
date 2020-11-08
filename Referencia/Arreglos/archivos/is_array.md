# is_array

Revisa si una variable es un _array_ o no.

## Sintaxis

  
```gml  
is_array(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|La variable a revisar.|  

## Descripción

Esta función revisa si una variable almacena un _array_ (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
a[7] = 0;  
if(is_array(a))  
    show_message("¡La variable ´a´ es un array!");  
```