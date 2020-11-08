# file_text_open_append

Abre un archivo de texto para añadirle información.

## Sintaxis

  
```gml  
file_text_open_append(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo a abrir.|  

## Descripción

Esta función permite abrir el archivo de texto dado para escribir contenido en él (si el archivo no existe, se creará) y automáticamente mueve el puntero al final del archivo, para que la escritura de contenido no reemplaze la información original, sino que se escriba después de ésta. Devuelve una identificación única, la cual debe almacenarse para poder realizar operaciones con el archivo. Si el archivo no existe, y no puede ser creado (debido a, por ejemplo, un nombre no válido) la función devolverá -1.  
  
**NOTA:** Sólo puede mantenerse un máximo de 32 archivos abiertos simultáneamente. Por ello, es necesario cerrar cada archivo una vez finalizado su uso, con el fin de liberar la memoria asociada e éste.

## Devuelve

Número real.

## Ejemplo

  
```gml  
f = file_text_open_append("Reporte.txt");  
file_text_write_string(f, "¡Hola! Este texto está escrito en este archivo gracias a GameMaker: Studio");  
file_text_close(f);  
```  
Se abre un archivo de texto para su escritura y se escribe en él una cadena de texto. Posteriormente, se cierra el archivo.