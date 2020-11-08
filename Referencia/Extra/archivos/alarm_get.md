# alarm_get

Obtiene el valor actual de la alarma solicitada.

## Sintaxis

  
```gml  
alarm_get(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice de la alarma que se desea obtener, de 0 a 11.|  

## Descripción

Esta función puede ser usada para obtener el valor actual de la alarma solicitada por el número argumentado. Esta función es una alternativa a usar directamente el _array_ `alarm`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
alarm[3] = 60;  
time = alarm_get(3); //Devuelve 60.  
```