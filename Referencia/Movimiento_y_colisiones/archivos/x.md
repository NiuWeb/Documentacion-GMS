# x

La posición horizontal de una instancia.

## Sintaxis

  
```gml  
x;  
```  

## Argumentos

Ninguno

## Descripción

La posición _x_ de una instancia es su posición horizontal en la sala actual, en pixeles. Este valor puede ser un número positivo, negativo o 0, donde 0 es el borde izquierdo de la sala; valores menores son más a la izquierda, y valores mayores a la derecha (un valor negativo significa que la instancia está por fuera del borde izquierdo de la sala). Es posible asignar cualquier número real al valor _x_, como 12.345, pero los valores decimales no parecerán tomados en cuenta.  
  
Modificando la posición de una instancia (`x` e `y`) es posible trasladarla a cualquier punto de la sala, o sumando/restando cantidades menores dar la impresión de movimiento sin utilizar las variables predefinidas `direction` y `speed`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(keyboard_check(vk_left))  
    x -= 5;  
if(keyboard_check(vk_right))  
    x += 5;  
```  
El código anterior permite mover una instancia horizontalmente, al presionar las teclas de dirección, con una velocidad de 5_px/step_.