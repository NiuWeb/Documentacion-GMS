# path_exists

Devuelve si existe un path con el índice dado o no.

## Sintaxis

  
```gml  
path_exists(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  

## Descripción

Esta función devuelve si existe un path o no con el índice dado. Tenga en cuenta que si hace la comprobación de un path con una variable no declarada, se producirá un error.

## Devuelve

Boleano

## Ejemplo

  
```gml  
if path_exists(path0){  
     path_start(path0, 4, path_action_reverse, 0);  
}  
```  
El código anterior comenzará el path0, si existe.