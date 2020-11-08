# path_get_x

Devuelve la coordenda en x de la posición dada de un path.

## Sintaxis

  
```gml  
path_get_x(index, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  
pos|La posición del path a obtener. Entre 0 (inicio) y 1 (final), acepta decimales.|  

## Descripción

Con esta función puede obtener la coordenada en X de una posición cualquiera del path dado. 0 es el inicio del path y 1 es el final del path; cualquier valor decimal intermedio a 0 y 1 equivale a una parte del path. Esto no necesita puntos definidos en el path.

## Devuelve

Número real

## Ejemplo

  
```gml  
x = path_get_x( path0, 0.5 );  
```  
El código anterior establece la posición en x de la instancia, a la coordenada en x de la posición media del path0.