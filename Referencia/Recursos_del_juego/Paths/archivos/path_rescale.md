# path_rescale

Escala el path dado con referencia su centro.

## Sintaxis

  
```gml  
path_rescale(index, xscale, yscale);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a escalar.|  
xscale|Por cuanto se multiplicará el tamaño horizontal. La escala predeterminada es 1.|  
yscale|Por cuanto se multiplicará el tamaño vertical. La escala predeterminada es 1.|  

## Descripción

Esta función puede ser usada para escalar el path dado en los dos ejes (o solamente uno), eje vertical y horizontal. Básicamente moviendo cada uno de los puntos del path a una nueva posición que corresponda, relativa al centro del path. Esta función cambia los datos del path de forma permanente desde que se usa hasta el final del juego, por lo que todas las instancias que usen del path se verán afectadas.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_rescale(path0, 3, 3);  
```  
El código anterior escalará "path0" a tres veces su tamaño original.