# path_insert_point

Inserta un punto en el path dado, en la posición indicada.

## Sintaxis

  
```gml  
path_insert_point(index, n, x, y, speed);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path en el que se insertara el punto.|  
n|La posición del nuevo punto, los puntos se desplazaran hacia delante.|  
x|La coordenada en x del nuevo punto (relativa al path).|  
y|La coordenada en y del nuevo punto (relativa al path).|  
speed|El factor de velocidad del punto.|  

## Descripción

Con esta función puede insertar un nuevo punto dentro del path (el path puede haber sido creado con el editor de path o mediante la función `path_add()`. El punto ha ser agregado en el path será antes del punto "n" especificado en la función.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_insert_point(mypath, 0, 50, 50, 100);  
```  
El código anterior inserta un punto al comienzo del path indexado en la variable "mypath" en (50, 50), con una velocidad del 100%.