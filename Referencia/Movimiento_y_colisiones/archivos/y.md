# y

La posición vertical de una instancia.

## Sintaxis

  
```gml  
y;  
```  

## Argumentos

Ninguno

## Descripción

La posición _y_ de una instancia es su posición vertical en la sala actual, definida en pixeles. Este valor puede ser un número positivo, negativo o 0. Donde 0 es el borde superior de la sala; valores menores son más hacia arriba, y valores mayores son hacia abajo (un valor negativo significa que la instancia está arriba (o afuera) del borde superior de la sala). Es posible asignar cualquier número real a la posición _y_, como 12.345, pero los valores decimales no parecerán tomados en cuenta.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(keyboard_check(vk_up))  
    y -= 5;  
if(keyboard_check(vk_down))  
    y += 5;  
```  
El código anterior permite mover una instancia verticalmente al presionar las teclas de dirección (arriba y abajo), con una velocidad de 5_px/step_.