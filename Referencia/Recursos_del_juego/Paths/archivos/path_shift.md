# path_shift

Desplaza el path dado a cualquier cantidad de pixeles horizontal y verticalmente.

## Sintaxis

  
```gml  
path_shift(index, xshift, yshift);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a cambiar.|  
xshift|El número de pixeles horizontales a desplazar el path. Negativo = izquierda, Positivo = derecha.|  
yshhift|El número de pixeles verticales a desplazar el path. Negativo = arriba, Positivo = abajo.|  

## Descripción

Con esta función puede desplazar el path a lo largo del eje horizontal y vertical. Tenga en cuenta que el cambio no será visible en le juego si la instancia sigue el path de forma relativa, ya que la posición del path no es tomada en cuenta. Esta función cambia los datos del path de forma permanente desde que se usa la función hasta el final del juego, por lo que todas las instancias que usen el path se verán afectadas.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_shift(mypath, 50, 50);  
```  
El código anterior desplaza el path0 50 pixeles a la derecha, y 50 pixeles abajo.