# ord

Devuelve el código Unicode del caracter dado.

## Sintaxis

  
```gml  
ord(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|El caracter al cual se desea obtener el código Unicode (Una cadena de solo un caracter). |  

## Descripción

Esta función devuelve el valor Unicode del caracter dado. Con esta función es posible, por ejemplo, almacenar caracteres como números enteros, o comprobar eventos de teclado con teclas de letras.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = ord("A"); //Devuelve 65.  
  
if(keyboard_check_pressed(a))  
    show_message("¡Se ha presionado la tecla 'A'!");  
```