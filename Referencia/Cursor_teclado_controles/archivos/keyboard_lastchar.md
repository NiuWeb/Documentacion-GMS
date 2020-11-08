# keyboard_lastchar

Almacena el ultimo caracter presionado (como una cadena de texto).

## Sintaxis

  
```gml  
keyboard_lastchar;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable almacena una cadena de texto del ultimo carácter presionado. Esta variable _no es_ de solo lectura, y puede cambiarla por ejemplo a "" (una cadena de texto vacía) con el fin de reiniciarla.

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
if keyboard_lastkey != -1{  
     str += keyboard_lastchar;  
     keyboard_lastkey = -1;  
}  
```  
Con el código anterior comprueba si la variable `keyboard_lastkey` es mayor a -1, si esto es verdadero agrega el ultimo carácter a la variable "str".