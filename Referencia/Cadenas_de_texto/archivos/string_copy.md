# string_copy

Devuelve una parte de una cadena de texto.

## Sintaxis

  
```gml  
string_copy(str, pos, count);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena de la cual copiar.|  
pos|La posición del primer caracter a obtener.|  
count|La cantidad de caracteres a obtener.|  

## Descripción

Con esta función es posible seleccionar una copia de una cadena. El primer caracter de una cadena se encuentra en la posición 1.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Hola mundo";  
a = string_copy(texto, 1, 1); //Devuelve 'H'  
a = string_copy(texto, 1, 4); //Devuelve 'Hola'  
a = string_copy(texto, 3, 5); //Devuelve 'la mu'  
```