# path_get_name

Devuelve el nombre del path dado.

## Sintaxis

  
```gml  
path_get_name(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  

## Descripción

Esta función devuelve el nombre del path en forma de una cadena de texto. El nombre es el definido en el editor de path ó (si el path a sido creado a través de funciones de código) este regresara una cadena de texto con el formato "_newpathXX" donde "XX" es el numero del path creado, empezando en 0 e incrementando de uno en uno cada vez que un path es creado. Tener en cuentra que este es una cadena de texto y no funciona para hacer referencia al path - para eso es necesario el _path index_. Puede usar la cadena de texto dada para obtener el _path index_ con la función `asset_get_index()`.

## Devuelve

Cadena de texto

## Ejemplo

  
```gml  
name = path_get_name(mypath);  
```  
El código anterior establece "name" con el nombre del path indexado en la variable "mypath".