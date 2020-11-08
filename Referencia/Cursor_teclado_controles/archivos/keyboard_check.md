# keyboard_check

Devuelve si la tecla dada está actualmente presionada.

## Sintaxis

  
```gml  
keyboard_check(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla a comprobar si esta actualmente presionada.|  

## Descripción

Con esta función puedes comprobar si una tecla esta siendo presionada o no. A diferencia de `keyboard_check_pressed` o `keyboard_check_released` que se activan solamente al presionar o soltar una tecla, esta función se activara a cada paso mientras la tecla este presionada.  

## Devuelve

Boleano

## Ejemplo

  
```gml  
if keyboard_check(vk_left){  
     x -= 5;  
}  
```  
El código anterior comprueba si la tecla _flecha izquierda_ esta siendo presionada, si esto es cierto, moverá la instancia 5 pixeles a la izquierda a cada paso mientras esto sea cierto.