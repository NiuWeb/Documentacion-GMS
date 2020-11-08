# ini_section_exists

Comprueba si una sección existe dentro de un archivo ini.

## Sintaxis

  
```gml  
ini_section_exists(section);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|El nombre de la sección a comprobar.|  

## Descripción

Esta función permite comprobar si una sección existe (en cuyo caso devolverá `true`) dentro del archivo ini actualmente abierto o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
ini_open("perfil.ini");  
if(ini_section_exists("datos"))  
    nombre = ini_read_string("datos", "nombre", "player");  
else show_message("No hemos podido encontrar información sobre tu cuenta.");  
ini_close();  
```