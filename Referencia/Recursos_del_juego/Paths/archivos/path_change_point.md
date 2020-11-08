# path_change_point

Cambia los valores de un punto existente en el path.

## Sintaxis

  
```gml  
path_change_point(index, n, x, y, speed);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path que contiene el punto a modificar.|  
n|El número del punto a modificar.|  
x|La nueva coordenada en x (relativa al path).|  
y|La nueva coordenada en y (relativa al path).|  
speed|El nuevo factor de velocidad.|  

## Descripción

Con esta función puede cambiar la posición y/o el factor de velocidad de cualquier punto previamente definido en el path (el path puede haber sido creado con el editor de path o utilizando el codigo `path_add`).

## Devuelve

Nada

## Ejemplo

  
```gml  
for(var i = 0; i < path_get_number(path0); i ++){  
     var px = path_get_point_x(path0, i) + 32 - random(64);  
     var py = path_get_point_y(path0, i) + 32 - random(64);  
     path_change_point(path0, i, px, py, 100);  
}  
```  
El código anterior, recorre todos los puntos del path indexado en la variable "path0" y re-posiciona todos los puntos en una posición aleatoria dentro de un área de 64x64 pixeles.