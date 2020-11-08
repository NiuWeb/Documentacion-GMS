# path_end

Finaliza el path que la instancia esta siguiendo.

## Sintaxis

  
```gml  
path_end();  
```  

## Argumentos

Ninguno

## Descripción

Usar esta función finalizará el path actual que esta ejecutando la instancia.

## Devuelve

Nada

## Ejemplo

  
```gml  
if place_meeting(x, y, all){ path_end(); }  
```  
El código anterior finalizará el path actual si la instancia detecta una colisión con cualquier instancia.