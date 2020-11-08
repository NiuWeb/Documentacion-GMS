# path_add

Agrega un path vació y regrese su índice.

## Sintaxis

  
```gml  
path_add();  
```  

## Argumentos

Ninguno

## Descripción

Con esta función puede crear un path en GameMaker: Studio sin usar el editor de path's, esta función regresa el índice del path para ser guardado dentro de una variable y usar dicha variable para manipular el path. Consideré que el path creado esta vació, es decir, no tiene puntos definidos y es necesario usar otras funciones para agregarlos o usar una `mp_grids` para generar el path. Al terminar de usar el path, o deseé crear otro dentro de la misma variable, primero debe de eliminar el path viejo con `path_delete` y así prevenir fugas de memoria que causarían el cierre de su juego.

## Devuelve

Número real

## Ejemplo

  
```gml  
global.newpath = path_add();  
```  
Con el código anterior se crea un nuevo path y se asigna su indice a la variable `global.newpath`