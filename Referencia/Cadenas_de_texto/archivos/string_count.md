# string_count

Devuelve el número de coincidencias de una subcadena encontradas en una cadena principal.

## Sintaxis

  
```gml  
string_count(substr, str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
substr|La cadena a buscar.|  
str|La cadena en donde buscar.|  

## Descripción

Esta función devuelve el número de veces que la subcadena dada aparece dentro de la cadena especificada.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
texto = "Un pequeño texto, dos pequeñas frases";  
  
a = string_count("e", texto); //Devuelve 6  
a = string_count("pequeñ", texto); //Devuelve 2  
a = string_count(" ", texto); //Devuelve 5  
a = string_count(",", texto); //Devuelve 1  
```