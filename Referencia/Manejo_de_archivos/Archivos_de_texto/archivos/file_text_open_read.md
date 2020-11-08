# file_text_open_read

Abre un archivo de texto para su lectura.

## Sintaxis

  
```gml  
file_text_open_read(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo de texto a abrir.|  

## Descripción

Esta función permite abrir el archivo de texto con el nombre dado para su posterior lectura. En caso exitoso, se devolverá una identificación única que debe almacenarse para poder ejecutar acciones con el archivo abierto; de lo contrario, devolverá -1.  
  
**NOTA:** Sólo puede mantenerse un máximo de 32 archivos abiertos simultáneamente. Por ello, es necesario cerrar cada archivo una vez finalizado su uso, con el fin de liberar la memoria asociada e éste.

## Devuelve

Número real.

## Ejemplo

  
```gml  
archivo = file_text_open_read("datos.ini");  
```