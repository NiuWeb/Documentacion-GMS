# path_get_closed

Devuelve el estado de la propiedad "closed" del path dado.

## Sintaxis

  
```gml  
path_get_closed(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  

## Descripción

Con esta función puede conocer si el path esta marcado como cerrado (true) o como abierto (false), es decir, si el path es un bucle o si tiene un comienzo y un final definidos.

## Devuelve

Boleano

## Ejemplo

  
```gml  
state = path_get_closed(c_path);  
```  
Se establecerá "state" en `true` o `false` dependiendo si el path indexado en "c_path" es cerrado o abierto.