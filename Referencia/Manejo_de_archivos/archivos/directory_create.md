# directory_create

Crea un directorio con el nombre dado.

## Sintaxis

  
```gml  
directory_create(dname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
dname|El nombre del directorio a crear.|  

## Descripción

Esta función crea un directorio con el nombre dado dentro del área local de guardado (_sandbox_).

## Devuelve

Nada

## Ejemplo

  
```gml  
directory_create("Levels/Downloaded_Games");  
```  
Se crea un directorio llamado **Downloaded_Games** en el directorio **Levels** dentro del área local de guardado (_sandbox_).