# file_find_next

Busca el siguiente archivo que cumpla con el patrón y los atributos dados.

## Sintaxis

  
```gml  
file_find_next();  
```  

## Argumentos

Ninguno

## Descripción

Esta función devuelve el nombre del siguiente archivo que cumpla con el patrón y los atributos previamente definidos (usando la función `file_find_first()`). Si no se encuentra ningún archivo, se devolverá una cadena vacía (`""`).  
  
**NOTA:** Esta función trabaja en todas las plataformas basadas en C++ (Windows, Mac, iOS, Android y Windows Phone), pero los atributos sólo funcionan en Windows o Windows Phone.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
primero = file_find_first("*.ini", 0);  
siguiente = file_find_next();  
```  
Se busca el primer archivo que tenga extensión .ini, y posteriormente se busca el siguiente archivo que cumpla esta misma condición.