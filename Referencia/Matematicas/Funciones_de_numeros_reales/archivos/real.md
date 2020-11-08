# real

Convierte una cadena de texto a un número real.

## Sintaxis

  
```gml  
real(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a convertir.|  

## Descripción

Esta función permite convertir una cadena de texto dada a un número real. En la conversión, los números, signos menos, puntos decimales y partes exponenciales de la cadena son tomadas en cuenta, mientras que otros caracteres (como letras) causarán un error. Si existe la posibilidad de que la cadena que se usará contenga caracteres no admitidos, se puede hacer uso de la función `string_digits()` para remover todos los caracteres no numéricos antes de realizar la conversión.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = "5";  
b = "32.5";  
  
ra = real(a); //Devuelve 5  
rb = real(b) + ra; //Devuelve 37.5  
r = real("-11.1"); //Devuelve -11.1  
```