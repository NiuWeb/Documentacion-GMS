# string_delete

Devuelve una copia de la cadena dada sin la selección establecida.

## Sintaxis

  
```gml  
string_delete(str, pos, count);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena de la cual copiar y eliminar.|  
pos|La posición del primer caracter de la selección.|  
count|La cantidad de caracteres de la selección.|  

## Descripción

Con esta función es posible eliminar una parte específica de una cadena. Se ingresa la cadena principal y los parámetros para establecer la selección de caracteres a eliminar (el primer caracter de una cadena es la posición 1), y la función devolverá una nueva cadena, sin dicha selección.  
  
**NOTA:** Esta función **no** modificará la cadena original, sólo devolverá una copia de la misma.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
texto = "Qué bonita vecindaaaaaad, es la vecindad del chavoooo";  
a = string_delete(texto, 5, 7); //Devuelve 'Qué vecindaaaaaad, es la vecindad del chavoooo'  
a = string_delete(texto, 18, 5); //Devuelve 'Qué bonita vecindad, es la vecindad del chavoooo'  
```