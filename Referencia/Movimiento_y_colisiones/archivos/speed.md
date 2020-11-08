# speed

La velocidad de la instancia.

## Sintaxis

  
```gml  
speed;  
```  

## Argumentos

Ninguno

## Descripción

Todas las instancias en _GameMaker: Studio_ poseen ciertas propiedades internas que pueden ser configuradas para personalizar su comportamiento. La variable `speed` es una de ellas, y permite definir la velocidad con la que una instancia se mueve hacia la dirección definida por `direction`. Esta variable acepta valores negativos, en cuyo caso la instancia se movería en dirección opuesta a la definida por `direction`.

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