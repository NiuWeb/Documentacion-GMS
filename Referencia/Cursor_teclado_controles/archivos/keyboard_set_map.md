# keyboard_set_map

Asigna a una tecla el valor de otra tecla.

## Sintaxis

  
```gml  
keyboard_set_map(key1, key2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key1|Esta es la tecla que recibirá un nuevo valor.|  
key2|Esta es la tecla que debe de ser asignada.|  

## Descripción

Esta función permite asignar a una tecla el valor de otra y la pulsación de estas teclas se interpretaran como el mismo. Para ello elige la tecla que desea asignar (key2) y la tecla a la cual se le asignará (key1).  
Con esta función puede crear un sistema en el cual el jugador defina sus propias teclas para jugar cómodamente su juego.

## Devuelve

Boleano

## Ejemplo

  
```gml  
keyboard_set_map(ord("A"), vk_left);  
```  
El código anterior, asignará a la tecla "A" el valor de la tecla `vk_left`. Esto significa que el jugador puede utilizara la tecla "A" o la tecla izquierda, y todo el código escrito para la flecha izquierda también responderá a la tecla "A".