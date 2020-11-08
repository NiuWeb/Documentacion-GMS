# path_scale

Establece (o devuelve) la escala del path.

## Sintaxis

  
```gml  
path_scale;  
```  

## Argumentos

Ninguno

## Descripción

Esta variable puede ser usada para establecer o devolver la escala del path actualmente asignado a la instancia, su valor por defecto es 1. Este valor de escala es de 1:1, si es establecido en 2, por ejemplo, se escalara al doble de su tamaño original.

## Devuelve

Número real

## Ejemplo

  
```gml  
path_scale = 1 + random(2);  
```  
El código anterior establecerá la escala del path actual a un valor aleatorio entre 1 (el tamaño original) y 3 (tres veces el tamaño original).