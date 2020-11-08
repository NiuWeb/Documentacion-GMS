# part_system_create

Crea un sistema de partículas y devuelve su índice.

## Sintaxis

  
```gml  
part_system_create();  
```  

## Descripción

Esta función crea un nuevo sistema de partículas y devuelve el índice único que debe ser almacenado en una variable y puede ser utilizado como argumento en otras funciones para hacer referencia a ese sistema.  
  
Los índices son números enteros. El primer sistema de partículas creado tiene índice 0 y los siguientes van incrementado en unidades.

## Devuelve

Entero (0, 1, 2,…)

## Ejemplo

  
```gml  
global.partsys1 = part_system_create();  
          
```  
En el ejemplo se crea un sistema de partículas y el índice se guarda en la variable global partsys1.