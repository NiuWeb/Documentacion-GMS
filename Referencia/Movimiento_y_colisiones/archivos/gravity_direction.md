# gravity_direction

La dirección a la cual aplicar la gravedad de una instancia.

## Sintaxis

  
```gml  
gravity_direction;  
```  

## Argumentos

Ninguno

## Descripción

Todas las instancias en _GameMaker: Studio_ poseen ciertas propiedades internas que pueden ser configuradas para personalizar su comportamiento. La variable gravity_direction es una de ellas, y permite definir la dirección en la cual la fuerza de gravedad, dada por la variable `gravity`, debe ser aplicada. Generalmente, 0º equivale a un movimiento hacia la derecha, 90º hacia arriba, 180º hacia la izquierda y 270º hacia abajo.

## Devuelve

Número real.

## Ejemplo

  
```gml  
gravity = 1;  
gravity_direction = 270;  
```  
Se aplicará una gravedad de 1 hacia abajo a la instancia.