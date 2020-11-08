# ini_write_string

Escribe una cadena de texto dentro de un archivo ini.

## Sintaxis

  
```gml  
ini_write_string(section, key, value);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ini en donde escribir el valor.|  
key|La llave en donde escribir el valor.|  
value|La cadena de texto a escribir.|  

## Descripción

Un archivo ini se compone de **secciones**, y dentro de cada una de ellas se encuentran parejas **llave=valor**. Un ejemplo de la estructura de un archivo ini es el siguiente:  
![](imagenes/ini_files.PNG)  
Donde las secciones se encuentran encerradas en corchetes ([ y ]), y cada llave posee en frente suyo su respectivo valor.  
  
Esta función permite escribir una cadena de texto en un archivo ini teniendo en cuenta la sección y la llave dadas. Si la sección establecida no existe, ésta se creará. Si la llave establecida no existe, ésta también se creará; de lo contrario, su valor será reemplazado.

## Devuelve

Nada.

## Ejemplo

  
```gml  
ini_open("datos.ini");  
ini_write_string("perfil", "usuario", "Albert");  
ini_close();  
```  
Se abre el archivo datos.ini y se escribe la cadena `"Albert"` dentro de la llave `"usuario"` de la sección `"perfil"` del archivo. Posteriormente se cierra el archivo.