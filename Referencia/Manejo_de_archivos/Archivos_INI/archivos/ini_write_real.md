# ini_write_real

Escribe un número real dentro de un archivo ini.

## Sintaxis

  
```gml  
ini_write_real(section, key, value);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ini en donde escribir el valor.|  
key|La llave en donde escribir el valor.|  
value|El número real a escribir.|  

## Descripción

Un archivo ini se compone de **secciones**, y dentro de cada una de ellas se encuentran parejas **llave=valor**. Un ejemplo de la estructura de un archivo ini es el siguiente:  
![](imagenes/ini_files.PNG)  
Donde las secciones se encuentran encerradas en corchetes ([ y ]), y cada llave posee en frente suyo su respectivo valor.  
  
Esta función permite escribir un número real en un archivo ini teniendo en cuenta la sección y la llave dadas. Si la sección establecida no existe, ésta se creará. Si la llave establecida no existe, ésta también se creará; de lo contrario, su valor será reemplazado.

## Devuelve

Nada.

## Ejemplo

  
```gml  
ini_open("datos.ini");  
ini_write_real("perfil", "nivel", 34);  
ini_close();  
```  
Se abre el archivo datos.ini y dentro de él se escribe el valor de 34 en la llave `"nivel"` dentro de la sección `"perfil"`. Posteriormente se cierra el archivo.