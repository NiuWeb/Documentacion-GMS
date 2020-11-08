# friction

La fricción a aplicarle a una instancia.

## Sintaxis

  
```gml  
friction;  
```  

## Argumentos

Ninguno

## Descripción

Todas las instancias en _GameMaker: Studio_ poseen ciertas propiedades internas que pueden ser configuradas para personalizar su comportamiento. La variable `friction` es una de ellas, y permite frenar o desacelerar la velocidad de una instancia. Su funcionamiento es muy simple: Por cada step que transcurra, se le resta el valor de esta variable a `speed`, si ésta es mayor a 0.

## Devuelve

Número real.

## Ejemplo

  
```gml  
friction = 1;  
```