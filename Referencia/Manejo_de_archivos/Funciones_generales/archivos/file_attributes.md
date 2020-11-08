# file_attributes

Comprueba si un archivo posee el atributo especificado.

## Sintaxis

  
```gml  
file_attributes(fname, attr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El archivo a examinar.|  
attr|El atributo a comprobar.|  

## Descripción

Esta función permite saber si un archivo dado posee el atributo dado. El atributo a comprobar puede ser una de las siguientes constantes:  

*   fa_readonly: Archivos de solo lectura.
*   fa_hidden: Archivos ocultos.
*   fa_sysfile: Archivos del sistema.
*   fa_volumeid: Archivos _volume-id_.
*   fa_directory: Directorios.
*   fa_archive: Archivados.

**NOTA:** Esta función sólo trabaja en Windows.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if(file_attributes("downloads/level03.ini", fa_readonly))  
    show_message("El archivo que intentas borrar está protegido (sólo lectura). La acción no se puede completar");  
```