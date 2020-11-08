# keyboard_check_pressed

Devuelve si la tecla dada ha sido presionada.

## Sintaxis

  
```gml  
keyboard_check_pressed(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla a comprobar si ha sido presionada.|  

## Descripción

Con esta función puedes comprobar si una tecla a sido presionada o no. A diferencia de la función `keyboard_check`, esta función es activada solo cuando es presionada la tecla, para volver a activarla es necesario soltar el botón y volver a presionarla.

## Devuelve

Boleano

## Ejemplo

  
```gml  
if keyboard_check_pressed(vk_anykey){  
   room_goto_next();  
}  
```  
El código anterior avanzará al siguiente cuarto si el jugador presionar cualquier tecla (Como para un mensaje de _**Presiona Cualquier Tecla para Continuar**_)