# gml_pragma

Establece cómo el YYC compila.

## Sintaxis

  
```gml  
gml_pragma(command);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
command|El comando a ejecutar (cadena de texto).|  

## Descripción

Esta función afecta la forma en la que el _YoYoCompiler_ compila el código del juego, y puede ser llamada utilizando diferentes comandos para modificar la compilación final del proyecto. Los comandos disponibles son:  
  
`"forceline"`: Cuando la función es llamada **en un script** utilizando este comando, el YYC compilará el proyecto de modo en que en donde el script se llame, se encuentre todo el código del mismo, y no la llamada a éste.

## Devuelve

Nada

## Ejemplo

  
```gml  
c = (argument0 + argument1)*(argument0/argument1);  
gml_pragma("forceline");  
return c;  
```  
Imaginemos que tenemos un script llamado `miscript()` que contiene el código anterior. Entonces, si desde un objeto cualquiera le llamamos así:  
```gml  
p = 32;  
h = 15.5;  
w = miscript(p, h);  
  
```  
Gracias al YYC, el código no sería compilado así, sino que quedaría de esta forma:  
```gml  
p = 32;  
h = 15.5;  
w = (32 + 15.5)*(32/15.5);  
  
```