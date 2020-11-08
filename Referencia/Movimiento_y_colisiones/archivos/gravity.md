# gravity

La gravedad a aplicarle a una instancia.

## Sintaxis

  
```gml  
gravity;  
```  

## Argumentos

Ninguno

## Descripción

Todas las instancias en _GameMaker: Studio_ poseen ciertas propiedades internas que pueden ser configuradas para personalizar su comportamiento. La variable `gravity` es una de ellas, y permite aplicar una fuerza constante en la dirección definida por `gravity_direction` de la instancia, influenciando la velocidad de la misma mediante la variable `speed`. Esta gravedad es una fuerza acumulativa, y por ello, acelerará la instancia gradualmente.  
  
El funcionamiento de esta variable es el siguiente: Por cada step que transcurra, se le añadirá el valor de gravity a speed, simulando un movimiento de caída en la dirección definida por `gravity_direction`.

## Devuelve

Número real.

## Ejemplo

  
```gml  
gravity = 1;  
gravity_direction = 270;  
```  
Se aplicará una gravedad de 1 hacia abajo a la instancia.