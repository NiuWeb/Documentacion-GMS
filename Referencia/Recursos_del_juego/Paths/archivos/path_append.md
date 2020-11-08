# path_append

Copia un path al final de otro path.

## Sintaxis

  
```gml  
path_append(index, path);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El nuevo índice del path.|  
path|El índice del path que se añadira a 'index'.|  

## Descripción

Con esta función puede añadir un path a otro, para que funcione correctamente deben existir ambos paths al momento de ejecutarlo (hechos con el editor de paths o creados con `path_add`).  
  
_**Nota:** Esta función no elimina el path que esta siendo agregado, solamente sus puntos son removidos, si ya no será utilizado, debe eliminarlo con la función `path_delete`._

## Devuelve

Nada

## Ejemplo

  
```gml  
path_append(mypath, mppath);  
path_delete(mppath);  
```  
El código anterior añade la información del path "mppath" a el path que se encuentra en la variable "mypath" y luego elimina "mppath" de la memoria.