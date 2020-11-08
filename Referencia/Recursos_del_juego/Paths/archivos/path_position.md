# path_position

La posición de la instancia dentro del path.

## Sintaxis

  
```gml  
path_position;  
```  

## Argumentos

Ninguno

## Descripción

Esta función puede ser usada para obtener o establecer la posición de una instancia a lo largo de un path. El valor debe ser entre 0 - 1, si establece el valor, por ejemplo, en 0.5, la instancia será colocada exactamente al medio del path.

## Devuelve

Número real

## Ejemplo

  
```gml  
path_position = random(1);  
```  
El código anterior establece una posición aleatoria en cualquier punto del path actual.