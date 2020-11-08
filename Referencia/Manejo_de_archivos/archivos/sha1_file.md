# sha1_file

Devuelve un _Hash SHA-1_ para el archivo dado.

## Sintaxis

  
```gml  
sha1_file(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo al cual obtener el Hash SHA-1.|  

## Descripción

SHA-1 es una función criptográfica de Hash diseñada por la Agencia de Seguridad Nacional de los Estados Unidos, y es implementada en muchas aplicaciones de seguridad. Esta función devuelve un mensaje de 160 bits (en formato ASCII) único para el archivo dado.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
file_hash = sha1_file("Created_Leveles/level07.ini");  
```  
Se obtiene un Hash SHA-1 para el archivo `"level07.ini"` que se encuentra dentro del directorio `"Created_Levels"`, y es almacenado en la variable `file_hash`.