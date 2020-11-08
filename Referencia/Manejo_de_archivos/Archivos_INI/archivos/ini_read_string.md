# ini_read_string

Lee una cadena de texto almacenada en un archivo ini.

## Sintaxis

  
```gml  
ini_read_string(section, key, def);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ini en donde se encuentra la cadena a leer.|  
key|La llave de la sección del archivo en donde se encuentra la cadena a leer|  
def|El valor por defecto (una cadena de texto) que se devolverá en caso de error.|  

## Descripción

Un archivo ini se compone de **secciones**, y dentro de cada una de ellas se encuentran parejas **llave=valor**. Un ejemplo de la estructura de un archivo ini es el siguiente:  
![](imagenes/ini_files.PNG)  
Donde las secciones se encuentran encerradas en corchetes ([ y ]), y cada llave posee en frente suyo su respectivo valor.  
  
Esta función permite obtener una cadena de texto almacenada dentro de la sección y la llave dados. En caso de que el archivo abierto, la sección o la llave dados no existan, se devolverá el valor por defecto establecido.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
ini_open("datos.ini");  
nombre = ini_read_string("perfil", "usuario", "Player");  
ini_close();  
```  
Se abre el archivo `"datos.ini"`. Posteriormente se lee la cadena almacenada en la llave usuario de la sección perfil, y por último se cierra el archivo. Si el archivo, la sección o la llave no existen, se devolverá `"Player"`.