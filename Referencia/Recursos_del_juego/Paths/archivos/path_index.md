# path_index

El índice del path que la instancia sigue actualmente.

## Sintaxis

  
```gml  
path_index;  
```  

## Argumentos

Ninguno

## Descripción

Todos los recursos de GameMaker: Studio poseen un identificador numérico único, la variable path_index es de **solo lectura** y almacena el índice del path asignado. Si la instancia no tiene un path asignado, la variable devolverá -1.

## Devuelve

ID

## Ejemplo

  
```gml  
if path_index = -1{  
     path_start(pth_enemy3, 4, path_action_reverse, 0);  
}  
```  
El codigo anterior comprueba si hay un path asigando a la instancia, si no es así comenzará un nuevo path. Asignando el índice del path a path_index al mismo tiempo).