# script_execute

Ejecuta un _script_ con los argumentos dados.

## Sintaxis

  
```gml  
script_execute(scr, [arg0, ..., arg14]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
scr|La identificación del script a ejecutar.|  
[arg0, ..., arg14]|La serie de argumentos (opcionales) con los cuales ejecutar el _script_.|  

## Descripción

Esta función permite ejecutar un script creado por el usuario e ingresarle hasta 15 argumentos. Es importante saber que el primer argumento **NO** es una cadena de texto, es el identificador del script como tal, como ha sido escrito en el recurso dentro del IDE.

## Devuelve

Valor devuelto por el script.

## Ejemplo

  
```gml  
//script(a, b);  
return (argument0+argument1)*(argument0/argument1);  
```  
Imaginemos que tenemos un script llamado `script()`, cuyo código es el anterior. Entonces:  
  
```gml  
a = script_execute(script, 3, 6); //Devuelve 4.5  
```