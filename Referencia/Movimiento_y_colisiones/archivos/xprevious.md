# xprevious

La posición horizontal previa de una instancia.

## Sintaxis

  
```gml  
xprevious;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable almacena la posición horizontal en la cual se encontraba la instancia en el _step_ anterior. Normalmente, el valor de esta variable cambia justo antes del inicio del evento _Begin Step_, aunque se le puede asignar manualmente cualquier valor.

## Devuelve

Número real.

## Ejemplo

  
```gml  
if(x != xprevious or y != yprevious)  
    show_message("La instancia se ha movido");  
```  
En el código anterior se puede comprobar si una instancia se ha movido tomando en cuenta su posición del _step_ anterior.