# room_height

La altura de la _room_ actual en píxeles.

## Sintaxis

  
```gml  
room_height;  
```  

## Descripción

Esta variable contiene la altura de la _room_ actual en píxeles. Puede cambiar esta variable para cambiar la altura de la _room_ en cualquier momento.

## Devuelve

Número Real

## Ejemplo

  
```gml  
if bbox_bottom > room_height  
    {  
    y += room_height - bbox_bottom;  
    }  
```  
El código anterior comprueba si el cuadro delimitador del _sprite_ de la instancia actual es mayor que la altura de la _room_, y si es así, ajusta la instancia al límite de la _room_.