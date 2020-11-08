# alarm_set

Establece el valor de una alarma.

## Sintaxis

  
```gml  
alarm_set(index, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice de la alarma a modificar. Un número de 0 a 11.|  
val|El valor a asignar.|  

## Descripción

Esta función puede ser utilizada para activar una alarma. Se ingresa el índice de la alarma (un número de 0 a 11) y el valor que se le asignará. El valor a asignar debe ser un número entero, y se puede asignar -1 para detener la alarma. Esta función es una alternativa a establecer el valor de la alarma directamente desde el array `alarm`.

## Devuelve

Nada.

## Ejemplo

  
```gml  
alarm_set(0, room_speed);  
```  
Se activa la alarma 0 para que se ejecute en un segundo.