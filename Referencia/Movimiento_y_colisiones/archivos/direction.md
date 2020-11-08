# direction

La dirección del movimiento de la instancia.

## Sintaxis

  
```gml  
direction;  
```  

## Argumentos

Ninguno

## Descripción

Todas las instancias en _GameMaker: Studio_ poseen ciertas propiedades internas que pueden ser configuradas para personalizar su comportamiento. La variable `direction` es una de esas propiedades, y permite definir la dirección del movimiento de la instancia, en grados, cuando la variable `speed` de ésta posee un valor diferente a 0. Generalmente, 0º equivale a un movimiento hacia la derecha, 90º hacia arriba, 180º hacia la izquierda y 270º hacia abajo.

## Devuelve

Número real.

## Ejemplo

  
```gml  
speed = 5;  
if(keyboard_check(vk_left))  
    direction += 5;  
if(keyboard_check(vk_right))  
    direction -= 5;  
  
```  
Gracias al código anterior, es posible mover una instancia cambiando su dirección mediante las teclas direccionales (izquierda y derecha), con una velocidad de 5_px/step_.