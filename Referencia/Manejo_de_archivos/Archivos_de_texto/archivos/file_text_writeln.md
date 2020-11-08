# file_text_writeln

Escribe una nueva línea en el archivo de texto dado.

## Sintaxis

  
```gml  
file_text_writeln(fid);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fid|La identificación del archivo de texto.|  

## Descripción

Esta función permite insertar un nuevo salto de línea dentro del archivo de texto dado.

## Devuelve

Nada.

## Ejemplo

  
```gml  
datos[0] = "Usuario 32";  
datos[1] = "Nivel 5";  
datos[2] = "Cristobal";  
num = array_length_1d(datos);  
  
f = file_text_open_write("datos.dat");  
for(i = 0; i < num; i++) {  
    file_text_write_string(f, datos[i]);  
    file_text_writeln(f);  
}  
file_text_close(f);  
```  
En el anterior ejemplo, se abre un archivo de texto para su escritura, y se escriben en él todos los valores del array dado. Posteriormente, se cierra el archivo.