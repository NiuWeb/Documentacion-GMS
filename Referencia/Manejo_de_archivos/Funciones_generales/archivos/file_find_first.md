# file_find_first

Obtiene el nombre del primer archivo que cumpla con el patrón dado y posea el atributo establecido.

## Sintaxis

  
```gml  
file_find_first(mask, attr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
mask|El patrón de búsqueda.|  
attr|El atributo que debe tener el archivo a buscar.|  

## Descripción

Esta función permite obtener el nombre del primer archivo que cumpla con el patrón de búsqueda dado y también posea el atributo especificado. Si no se encuentra ningún archivo, se devolverá una cadena vacía (`""`). Por ejemplo, el patrón `"Levels/*.ini"` permite buscar todos los archivos con la extensión `".ini"` dentro del directorio Levels. El atributo indica los archivos adicionales que se deseen buscar; además, los archivos normales son siempre tomados en cuanda si éstos cumplen con el patrón. El atributo puede ser una de las siguientes constantes (si no se desea utilizar ningún atributo, usar 0):  

*   fa_readonly: Archivos de solo lectura.
*   fa_hidden: Archivos ocultos.
*   fa_sysfile: Archivos del sistema.
*   fa_volumeid: Archivos _volume-id_.
*   fa_directory: Directorios.
*   fa_archive: Archivados.

NOTA: Esta función no trabaja en plataformas JS (**HTML5**, **Tizen** y **Windows8**), y los atributos sólo funcionan en **Windows** y **Windows Phone** (utilizar 0 para las demás plataformas).

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
ini = file_find_first("Archivos/*.ini", 0); //Busca el primer archivo con extensión '.ini'  
anything = file_find_first("Niveles/*", fa_directory); //Busca el primer archivo o directorio  
file = file_find_first("Niveles/*.*", 0); //Busca el primer archivo con cualquier extensión  
```