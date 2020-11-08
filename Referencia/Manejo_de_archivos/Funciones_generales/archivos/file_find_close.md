# file_find_close

Finaliza la búsqueda de archivos y libera la memoria.

## Sintaxis

  
```gml  
file_find_close();  
```  

## Argumentos

Ninguno

## Descripción

Después del uso de las funciones `file_find_first()` y `file_find_next()`, esta función debe llamarse para eliminar de la memoria la búsqueda de archivos.

## Devuelve

Nada.

## Ejemplo

  
```gml  
archivo = file_find_first("*.ini", 0);  
file_find_close();  
```  
Se realiza una búsqueda del primer archivo que cumpla con el patrón dado, y al terminar, se libera la memoria.