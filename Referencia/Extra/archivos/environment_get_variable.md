# environment_get_variable

Devuelve el valor de una variable de entorno.

## Sintaxis

  
```gml  
environment_get_variable(name);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
name|El nombre de la variable de entorno (una cadena de texto).|  

## Descripción

Esta función devuelve el valor (una cadena de texto) de la variable de entorno con el nombre dado.  
  
**NOTA:** Esta función sólo trabaja en la plataforma Windows.

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
appdata = environment_get_variable("APPDATA");  
```  
Se obtiene el valor de la variable de entorno `"%appdata%"`, que en Windows Vista/7 equivale normalmente a `"C:Users{usuario}AppDataRoaming"`.