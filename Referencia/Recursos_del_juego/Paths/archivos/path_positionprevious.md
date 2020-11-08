# path_positionprevious

La posición de la instancia dentro del path en el step anterior.

## Sintaxis

  
```gml  
path_positionprevious;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable puede ser usada para obtener o establecer la posición de una instancia a lo largo del path en el step anterior, siendo este un valor entre 0 y 1. Es similar a las funciones de `xprevious` y `yprevious` solamente que es exclusiva para path. Puede ser útil para detener temporalmente a una instancia si algo esta en el camino (ejemplo a continuación).

## Devuelve

Número real

## Ejemplo

  
```gml  
var xx, yy;  
xx = x + lengthdir_x(16, direction);  
yy = y + lengthdir_y(16, direction);  
if collision_circle(xx, yy, 16, obj_Player, false,true)  
    path_position = path_positionprevious;  
```  
EL código anterior comprueba el área de enfrente de la instancia, por una colisión con el objeto "obj_Player" y si esto es cierto, la instancia volverá a su posición anterior que ocupaba en el actual path.