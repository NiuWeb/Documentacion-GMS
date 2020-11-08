# md5_file

Devuelve un _Hash MD5_ para el archivo dado.

## Sintaxis

  
```gml  
md5_file(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo al cual generar un _Hash MD5_.|  

## Descripción

En criptografía, MD5 (Message-Digest algorithm 5) es una función criptográfica de Hash con un hash de 128-bit extensamente usada en diferentes aplicaciones de seguridad. Esta función permite generar un MD5 único para el archivo.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
hash = md5_file("Checkpoints/save3.ini");  
```