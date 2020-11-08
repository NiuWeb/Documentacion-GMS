# int64

Intenta convertir un valor dado en un entero de 64 bits.

## Sintaxis

  
```gml  
int64(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El valor a intentar convertir.|  

## Descripción

Esta función intenta convertir un valor dado en un entero de 64 bits, donde el valor dado puede ser un real, una cadena, un entero de 64bits, un entero de 32 bits o un puntero. Cualquier otro tipo de valor producirá un error. Además, es posible verificar si una variable almacena un entero de 64 bits utilizando la función `is_int64()`.

## Devuelve

Número entero de 64 bits.

## Ejemplo

  
```gml  
val = int64("30"); //Devuelve 30 (número, no cadena)  
val2 = int64("25xyz"); //Devuelve 25 (número, no cadena)  
val3 = int64("19.31"); //Devuelve 19 (número, no cadena)  
```