# keyboard_clear

Limpia el estado de la tecla dada.

## Sintaxis

  
```gml  
keyboard_clear(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla a limpiar.|  

## Descripción

Con esta función puedes limpiar el estado actual del teclado, la utilidad es que si una tecla esta siendo presionada, deja de reconocerse hasta que sea soltada (Al utilizar esta función no se genera el evento `keyboard_key_release`) y presionada de nuevo.

## Devuelve

Nada

## Ejemplo

  
```gml  
keyboard_clear(vk_space);  
```  
Este código limpia el esta de la barra de espacio.