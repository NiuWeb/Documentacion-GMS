# path_rotate

Rota el path dado con relación a su centro.

## Sintaxis

  
```gml  
path_rotate(index, angle);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a rotar.|  
angle|El ángulo de rotación en grados.|  

## Descripción

Puede usar esta función para rotar el path dado con relación a su centro. Recuerde que en GameMaker: Studio (sin usar físicas) los ángulos se calculan al contrario de las agujas del reloj, por lo que establecer la orientación del path en 90, girará el path actual hacia la izquierda. Esta función modifica los datos del path permanentemente, desde que se usa la función hasta el final del juego, por lo que todas las instancias que usen el path se verán afectadas.

## Devuelve

Nada

## Ejemplo

  
```gml  
path_rotate(path0, 90);  
```  
El código anterior rota el path0 grados al contrario de las agujas del reloj.