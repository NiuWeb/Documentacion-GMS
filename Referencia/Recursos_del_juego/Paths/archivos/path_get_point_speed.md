# path_get_point_speed

Devuelve la velocidad establecida de un punto del path dado.

## Sintaxis

  
```gml  
path_get_point_speed(index, n);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  
n|El número del punto a comprobar.|  

## Descripción

Con esta función puede obtener la velocidad de un punto (tal como fue definido con el editor de path o agregado dinámicamente el punto usando `path_add_point()`) expresando en forma de porcentaje. Por ejemplo, si tiene un punto en el path con una velocidad de 50 en el editor de path, esta función devolverá 50 al ser utilizada.

## Devuelve

Número real

## Ejemplo

  
```gml  
if path_get_point_speed(c_path, 0) != 100{  
     path_change_point(c_path, 0, path_get_point_x(c_path, 0), path_get_point_y(c_path, 0), 100);  
}  
```  
El código anterior comprueba si la velocidad del punto "0" del path indexado en "c_path" no es igual a 100. Si no es 100, entonces la velocidad será establecida a 100.