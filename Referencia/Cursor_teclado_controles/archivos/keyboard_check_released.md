# keyboard_check_released

Devuelve si la tecla dada ha sido soltada.

## Sintaxis

  
```gml  
keyboard_check_released(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla a comprobar si ha sido soltada.|  

## Descripción

Con esta función puedes comprobar si una tecla a sido soltada o no. A diferencia de la función `keyboard_check`, esta función solo es activada cuando la tecla es soltada, si quiere volver a activarse es necesario presionarla primero para luego soltarla.

## Devuelve

Boleano

## Ejemplo

  
```gml  
if keyboard_check_released(ord('P')){  
     instance_create(0, 0, obj_Pause);  
}  
```  
El código anterior comprueba si la tecla ¨P¨ a sido soltada, si es cierto crea la instancia ¨obj_Pause¨.