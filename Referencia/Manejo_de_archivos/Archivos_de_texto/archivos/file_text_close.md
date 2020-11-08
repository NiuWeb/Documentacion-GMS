# file_text_close

Cierra el archivo de texto dado.

## Sintaxis

  
```gml  
file_text_close(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo a cerrar.|  

## Descripción

Al terminar de trabajar con un archivo de texto, es necesario cerrarlo, ya que de lo contrario se corre el riesgo de producirse pérdidas de información, como por ejemplo que el contenido escrito en el archivo no se guarde. Esta función previene saturaciones de memoria y problemas con el límite del sistema de archivos.  
  
Cabe mencionar que es posible mantener sólo hasta 32 archivos de texto abiertos simultáneamente, por lo que el uso de esta función es necesario para evitar errores.

## Devuelve

Nada.

## Ejemplo

  
```gml  
contenido = "";  
file = file_text_open_read("datos/partida1.ini");  
while(!file_text_eof(file)) {  
    contenido += file_text_read_string(file) + chr(13) + chr(10);  
    file_text_readln(file);  
}  
file_text_close(file);  
```  
En el ejemplo anterior, se abre un archivo de texto y se guarda su contenido en la variable `contenido`. Posteriormente se cierra el archivo.