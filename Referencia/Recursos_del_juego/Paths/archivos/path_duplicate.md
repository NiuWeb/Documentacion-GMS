# path_duplicate

Duplica un path existente, regresando su índice.

## Sintaxis

  
```gml  
path_duplicate(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path existente a duplicar.|  

## Descripción

Esta función toma un path y lo copia dentro de un nuevo path. El nuevo path es creado en el proceso, y el índice es guardado en una variable para las llamadas posteriores del nuevo path.

## Devuelve

Número real

## Ejemplo

  
```gml  
mypath = path_duplicate(choose(path_1, path_2, path_3, path_4));  
```  
El código anterior elige uno de los cuatro posibles paths y lo duplica, el índice del nuevo path es guardado en la variable "mypath".