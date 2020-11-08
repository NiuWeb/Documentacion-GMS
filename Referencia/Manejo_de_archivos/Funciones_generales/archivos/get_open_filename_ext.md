# get_open_filename_ext

Abre un cuadro de diálogo personalizado para cargar un archivo.

## Sintaxis

  
```gml  
get_open_filename_ext(filter, fname, dir, caption);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
filter|El filtro del archivo a cargar.|  
fname|El nombre sugerido del archivo.|  
dir|El directorio inicial del cuadro de diálogo.|  
caption|El título de la ventana del cuadro de diálogo.|  

## Descripción

Esta función abre un cuadro de diálogo en donde el jugador podrá elegir un archivo cuyo nombre coincida con el filtro dado. El filtro posee la forma `"Nombre 1|formato1|nombre2|formato2..."`. Donde el formato contiene los diferentes nombres que puede tener el archivo a elegir, separados por _punto y coma_; el asterisco (*) indica que se puede tratar de cualquier nombre. Cabe mencionar que esta función **no abre el archivo para leerlo**. Sólo devuelve una cadena de texto con la ruta y nombre completo del archivo que se ha abierto. Si el usuario cancela la operación (dígase presiona **Cancel**, o cierra el cuadro de diálogo), la función devolverá una cadena de texto vacía (`""`).  
  
Si el directorio inicial establecido no existe, el cuadro de diálogo se abrirá en la ruta predeterminada del sistema.  
  
Es importante saber que, a pesar del límite del sistema de archivos de GameMaker: Studio (que normalmente impide administrar archivos fuera del área local), esta función otorga permisos de lectura para el archivo abierto durante el resto del juego. Gracias a esto, es posible leer el contenido de un archivo abierto por esta función.  
  
**NOTA:** Esta función es sólo para la plataforma **Windows**.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file = get_open_filename_ext("Archivo INI|*.ini", "partida.ini", "C:DocumentsMyGamePartidas", "Seleccionar partida");  
file2 = get_open_filename_ext("Imagen|*.png;*.jpg|Archivo de texto|*.txt;*.ini", "", "C:DocumentsMyGamePartidas", "Seleccionar archivo a subir");  
```