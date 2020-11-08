# ini_key_exists

Comprueba si una llave existe en un archivo ini.

## Sintaxis

  
```gml  
ini_key_exists(section, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ini en donde buscar la llave.|  
key|La llave a buscar.|  

## Descripción

Esta función permite comprobar si una llave existe en el archivo ini abierto actualmente (en cuyo caso devolverá `true`) o no (en cuyo caso devolverá `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
ini_open("perfil.ini");  
if(ini_key_exists("perfil", "usuario"))  
    usuario = ini_read_string("perfil", "usuario");  
else {  
    show_message("No hemos encontrado un nombre de usuario para tu perfil. Por el momento usaremos uno automático");  
    usuario = "Albert";  
}  
ini_close();  
```