# string_format

Convierte un número real a una cadena de texto con propiedades personalizadas.

## Sintaxis

  
```gml  
string_format(val, int, dec);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número real a convertir.|  
int|El mínimo número de cifras enteras que se convertirán.|  
dec|El número de cifras decimales que se convertirán.|  

## Descripción

Esta función convierte un número real a una cadena de texto utilizando un formato propio. Si la cantidad de cifras enteras es menor al mínimo de éstas a convertir (argumento `int`), las cifras faltantes se llenarán con espacios de izquierda a derecha. Si el número de cifras decimales es menor al mínimo de éstas a convertir (argumento `dec`), las cifras faltantes se llenarán con ceros.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
a = 123.5678;  
b = string_format(a, 3, 4); //Devuelve '123.5678'  
b = string_format(a, 1, 4); //Devuelve '123.5678'  
b = string_format(a, 2, 3); //Devuelve '123.568'  
b = string_format(a, 4, 4); //Devuelve ' 123.5678'  
b = string_format(a, 5, 6); //Devuelve '  123.567800'  
b = string_format(a, 3, 1); //Devuelve '123.6'  
```