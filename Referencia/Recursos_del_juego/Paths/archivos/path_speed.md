# path_speed

La velocidad de la instancia con la que sigue al path(en pixeles por step).

## Sintaxis

  
```gml  
path_speed;  
```  

## Argumentos

Ninguno

## Descripción

Puede usar esta función para obtener o establecer la velocidad de un path después de ser iniciado. Si es usado un valor negativo, hará que la instancia ira de retroceso en el path.

## Devuelve

Número real

## Ejemplo

  
```gml  
path_speed = -1 + random(2);  
```  
El código anterior establece la velocidad con que recorrerá la instancia el path, en un valor aleatorio entre -1 y 1.