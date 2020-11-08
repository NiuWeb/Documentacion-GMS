# surface_free

Destruye la surface, liberándola de la memoria.

## Sintaxis

  
```gml  
surface_free(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a liberar.|  

## Descripción

Cuando se trabaja con surface, siempre se debe de usar esta función cada vez que se utilicen. Las surfaces ocupan espacio en la memoria y necesitan ser removidas, normalmente al finalizar una habitación, pero puede hacerse en cualquier momento dependiendo del uso que se les de. Si no lo hace causará perdidas de memoria que eventualmente ralentizarán y bloquearán su juego.  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Nada

## Ejemplo

  
```gml  
if keyboard_check_pressed(vk_escape){  
     surface_free(surf);  
     room_goto(rm_Menu);  
}  
```  
El código anterior comprueba si una tecla es presionada, si es así libera la memoria reservada para la surface indexada en la variable "surf" y luego cambia de room.