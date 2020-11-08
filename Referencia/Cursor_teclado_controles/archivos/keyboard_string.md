# keyboard_string

Mantiene una cadena de texto de las ultimas teclas presionadas.

## Sintaxis

  
```gml  
keyboard_string;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable mantiene una cadena de texto de los últimos caracteres escritos con el teclado (como máximo 1024). Esta cadena solo acepta caracteres imprimibles, pero responde correctamente a la tecla de borrado, para eliminar el último carácter. Esta variable **no es** de sólo lectura y puede ser modificada, por ejemplo para establecerla en "" (cadena de texto vacía) y utilizar _funciones de cadenas de texto_ para manipularla.

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
if string_length(keyboard_string) > 15{  
     keyboard_string = string_copy(keyboard_string, 1, 15);  
}  
```  
El código anterior limita el tamaño de la variable `keyboard_string` a solo 15 caracteres, removiendo todos los que se encuentren después al hacer una copia de solo los primeros 15 dentro de si mismo.