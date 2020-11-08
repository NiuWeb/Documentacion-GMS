# part_system_exists

Revisa si un sistema de partículas existe.

## Sintaxis

  
```gml  
part_system_exists(ind);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ind|Índice del sistema de partículas a revisar.|  

## Descripción

Con esta función se puede comprobar si un sistema de partículas existe. Normalmente se usa una variable como argumento, cuyo valor fue asignado previamente con la función `part_system_create()`.

## Devuelve

Devuelve: Booleano (true o false)

## Ejemplo

  
```gml  
if !part_system_exists(global.partsys1)  
{  
   global.partsys1 = part_system_create();  
}  
          
```  
En este código, si el sistema de partículas referenciado en la variable global no existe, se crea un nuevo sistema de partículas.