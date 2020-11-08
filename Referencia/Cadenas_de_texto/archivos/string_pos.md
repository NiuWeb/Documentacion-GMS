# string_pos

Devuelve la posición de una subcadena en la cadena dada.

## Sintaxis

  
```gml  
string_pos(substr, str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
substr|La subcadena a buscar.|  
str|La cadena en donde buscar.|  

## Descripción

Esta función devuelve la posición de la primera coincidencia de una subcadena en la cadena dada. Si no se encuentra ninguna coincidencia, devolverá 0.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
texto = "correo@electronico.com";  
arroba = string_pos("@", texto); //Devuelve 7  
if(arroba != 0)  
    show_message("¡Correo electrónico válido!");  
```