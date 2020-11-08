# path_get_y

Devuelve la coordenada en y de la posición dada de un path.

## Sintaxis

  
```gml  
path_get_y(index, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  
pos|La posición del path a obtener. Entre 0 (inicio) y 1 (final), acepta decimales.|  

## Descripción

Con esta función puede obtener la coordenada en Y de una posición cualquiera del path dado. 0 es el inicio del path y 1 es el final del path; cualquier valor decimal intermedio a 0 y 1 equivale a una parte del path. Esto no necesita puntos definidos en el path.

## Devuelve

Número real

## Ejemplo

  
```gml  
y = path_get_y( path0, 0.5 );  
```  
El código anterior establece la posición en y de la instancia, a la coordenada en y de la posición media del path0.