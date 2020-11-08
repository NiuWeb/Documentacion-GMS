# path_get_speed

Devuelve el factor de velocidad del

## Sintaxis

  
```gml  
path_get_speed(index, pos);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  
pos|La posición del path a comprobar. Entre 0 (inicio) y 1 (final), acepta decimales.|  

## Descripción

Esta función devuelve el factor de velocidad de cualquier posición del path dado. La posición debe ser un valor entre 0 y 1 (puede usar `path_position`, por ejemplo, si desea usar la posición actual de la instancia) siendo 0 la posición de inicio y 1 el final. El valor que se devuelve es la velocidad media entre los puntos que se encuentra la posición dada. Ejemplo, si un path tiene solo 2 puntos, el punto 0 posee 100 de velocidad y el punto 1 0, la función path_get_speed(path, 0.5) devolverá 50.

## Devuelve

Real

## Ejemplo

  
```gml  
speed = path_get_speed(path0, 0.5) / 20;  
```  
El código anterior establecerá la velocidad de la instancia, al factor de velocidad de la posición media del path0, dividida entre 20. Si el factor de velocidad es de 100, la velocidad de la instancia será 5.