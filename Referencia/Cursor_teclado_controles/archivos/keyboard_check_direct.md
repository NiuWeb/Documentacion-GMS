# keyboard_check_direct

Comprueba si la tecla dada es presionada, verificando el hardware directamente.

## Sintaxis

  
```gml  
keyboard_check_direct(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla a comprobar si ha sido presionada.|  

## Descripción

Esta función regresa _true_ si la tecla especificada a sido presiona, o _false_ si no, comprobando el hardware directamente. Permite el uso de constantes **vk_** adicionales: `vk_lshift, vk_lcontrol, vk_lalt, vk_rshift, vk_rcontrol, vk_ralt` para comprobar si las teclas del lado izquierdo o derecho son presionadas.  
_**Nota:** Esta función solo esta disponible para Windows estándar, es resultado es independiente de la plataforma seleccionada._

## Devuelve

Boleano

## Ejemplo

  
```gml  
if keyboard_check_direct(vk_ralt) || keyboard_check_direct(vk_lalt){  
      crouch = true;  
}  
```  
El código anterior comprueba si la tecla **alt** del lado izquierdo o derecho es presionada, si es correcto el valor de la variable "crouch" pasa a ser true.