# path_reverse

Invierte el path dado.

## Sintaxis

  
```gml  
path_reverse(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a modificar.|  

## Descripción

Con esta función puede invertir el orden individual de un path en que se enumeran los puntos. Por ejemplo en un path de 5 puntos, enumerados desde el 0 hasta el 4, el punto 1 pasará a ser el 3 y el punto 2 se mantendrá. La posición de los puntos se mantendrá, solo se cambia el orden en que estos son procesados. Esta función modifica los datos del path, desde que la función es utilizada hasta el final del juego, por lo que todas las instancias que usen el path se verán afectadas.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_reverse(path0);  
```  
El código anterior invierte el orden en que son procesados todos los puntos del path indexado en "path0".