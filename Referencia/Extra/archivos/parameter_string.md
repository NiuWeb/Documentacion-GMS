# parameter_string

Devuelve el parámetro de línea de comando ubicado en el índice dado.

## Sintaxis

  
```gml  
parameter_string(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del parámetro de línea de comando a obtener.|  

## Descripción

Los parámetros de línea de comandos son información extra que se puede agregar a un programa cuando se es ejecutado. Esta función permite obtener uno de esos parámetros; más específicamente, el ubicado en el índice dado.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
var i, parametro;  
for(i = 1; i <= parameter_count(); i++)  
    parametro[i] = parameter_string(i);  
```  
Se insertan todos los parámetros de línea de comandos que hayan en el _array_ `parametro`.