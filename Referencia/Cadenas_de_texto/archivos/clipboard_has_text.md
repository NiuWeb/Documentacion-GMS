# clipboard_has_text

Comprueba si el portapapeles del dispositivo tiene contenido.

## Sintaxis

  
```gml  
clipboard_has_text();  
```  

## Argumentos

Ninguno

## Descripción

Esta función devuelve `true` si el portapapeles del dispositivo contiene texto, o `false` si está vacío.  
  
**NOTA:** Esta función es válida sólo para la plataforma **Windows**.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if(clipboard_has_text())  
    clipboard_set_text("");  
```  
Si el portapapeles del dispositivo contiene texto, limpiarlo.