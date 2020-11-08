# get_save_filename

Abre un cuadro de diálogo que permite guardar un archivo.

## Sintaxis

  
```gml  
get_save_filename(filter, fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
filter|El filtro de archivo a guardar.|  
fname|El nombre sugerido del archivo.|  

## Descripción

Esta función abre un cuadro de diálogo en donde el jugador podrá guardar un archivo cuyo nombre coincida con el filtro dado. El filtro posee la forma `"Nombre 1|formato1|nombre2|formato2..."`. Donde el formato contiene los diferentes nombres que puede tener el archivo a elegir, separados por _punto y coma_; el asterisco (*) indica que se puede tratar de cualquier nombre. Cabe mencionar que esta función **no abre el archivo para su escritura**. Sólo devuelve una cadena de texto con la ruta y nombre completo del archivo guardado. Si el usuario cancela la operación (dígase presiona **Cancel**, o cierra el cuadro de diálogo), la función devolverá una cadena de texto vacía (`""`).  
  
Es importante saber que, a pesar del límite del sistema de archivos de GameMaker: Studio (que normalmente impide administrar archivos fuera del área local), esta función otorga permisos de escritura para el archivo guardado durante el resto del juego. Gracias a esto, es posible modificar el contenido de un archivo abierto por esta función.  
  
**NOTA:** Esta función es sólo para la plataforma **Windows**.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = get_save_filename("Archivo INI|*.ini|Archivo JSON|*.json|Archivo binario|*.bin", program_directory);  
  
h = file_text_open_write(file);  
file_text_write_string(h, "Este es un archivo que el usuario ha guardado");  
file_text_close(h);  
```  
Se abre un cuadro de diálogo que permite al usuario guardar un archivo, y elegir entre hacerlo con formato INI, JSON o binario. Por defecto, el cuadro de diálogo se abre en la ruta en donde se encuentra el ejecutable, y posteriormente, se escribe contenido en el archivo guardado.