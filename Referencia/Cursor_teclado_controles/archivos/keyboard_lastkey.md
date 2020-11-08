# keyboard_lastkey

Almacena el codigo de la ultima tecla presionada.

## Sintaxis

  
```gml  
keyboard_lastkey;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable contiene el valor de `keyboard_key` del cuadro anterior, regresando el código asignado a la tecla (todos los códigos de las constantes estándares son devueltos). Esta variable _no es_ de solo lectura y puede ser cambiada, por ejemplo a -1 para "reiniciarla".

## Devuelve

Entero

## Ejemplo

  
```gml  
if (keyboard_lastkey != -1){  
     str += keyboard_lastchar;  
     keyboard_lastkey = -1;  
}  
```  
El código anterior comprueba si la variable `keyboard_lastkey` no es igual a -1, si esto es verdadero agrega la ultima tecla como una cadena de texto a la variable "str", luego reinicia la variable `keyboard_lastkey` para permitir una futura comprobación.