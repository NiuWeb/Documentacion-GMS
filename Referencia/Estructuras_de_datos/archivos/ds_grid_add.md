# ds_grid_add

Añade un valor a una celda dentro del a grid.

## Sintaxis

  
```gml  
ds_grid_add(index, x, y, val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice de la grid.|  
x|La posición en x de la celda dentro de la grid.|  
y|La posición en y de la celda dentro de la grid.|  
val|El valor a añadir a la celda.|  

## Descripción

Esta función puede ser usada para agregar un valor dado (número real o cadena de texto) a el valor de la celda dada dentro de la grid. El valor a agregar debe de ser del mismo tipo que contiene la celda, ejemplo: no puedes añadir una cadena de texto a un número real y viceversa, para las cadenas de texto esto corresponde a la concatenación.

## Devuelve

Nada

## Ejemplo

  
```gml  
ds_grid_add(grid, 5, 5, 6);  
```  
El código anterior añade 6 a la celda dada dentro de la grid indexada en la variable "grid".