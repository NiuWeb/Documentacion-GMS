# room_width

La anchura de la _room_ actual en píxeles.

## Sintaxis

  
```gml  
room_width;  
```  

## Descripción

Esta variable contiene la anchura de la _room_ actual en píxeles. Puede cambiar esta variable para cambiar la anchura de la _room_ en cualquier momento.

## Devuelve

Número Real

## Ejemplo

  
```gml  
if bbox_right > room_width  
    {  
    x += room_width - bbox_right;  
    }  
```  
El código anterior comprueba si el cuadro delimitador del _sprite_ de la instancia actual es mayor que la anchura de la _room_, y si es así, ajusta la instancia al límite de la _room_.