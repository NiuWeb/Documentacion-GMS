# external_call

Llama a una función externa previamente definida.

## Sintaxis

  
```gml  
external_call(name, args[1, ..., 15]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
name|El nombre de la función externa a llamar (cadena de texto).|  
args[1, ..., 15]|Los diferentes valores que se desean enviar como argumentos a la función externa.|  

## Descripción

Si se ha creado una función externa desde una _dll_ o _dylib_ utilizando `external_define()`, es posible utilizar esta función para llamarla. Se argumenta el nombre de la función previamente definida y los argumentos que se desan enviar (cada argumento debe concordar con el tipo de dato seleccionado al crearse la función).  
  
Esta función devuelve el resultado que devuelve función externa llamada.

## Devuelve

Cadena de texto o número real.

## Ejemplo

  
```gml  
a = external_call("mi_funcion", 2, 4); //Se llama a la función externa 'mi_funcion' con los números 2 y 4 como argumentos.  
```