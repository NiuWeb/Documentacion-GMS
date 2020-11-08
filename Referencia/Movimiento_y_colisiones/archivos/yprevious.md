# yprevious

La posición vertical previa de una instancia.

## Sintaxis

  
```gml  
yprevious;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable almacena la posición vertical en la cual se encontraba la instancia en el _step_ anterior. Normalmente, el valor de esta variable cambia justo antes del inicio del evento _Begin Step_, aunque se le puede asignar manualmente cualquier valor.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(x != xprevious or y != yprevious)  
    show_message("La instancia se ha movido");  
```  
En el código anterior se puede comprobar si una instancia se ha movido tomando en cuenta su posición del step anterior.