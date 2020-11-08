# path_get_number

Devuelve el número de puntos de un path.

## Sintaxis

  
```gml  
path_get_number(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  

## Descripción

Esta función puede ser usada para obtener el número de puntos de un path.

## Devuelve

Número real

## Ejemplo

  
```gml  
if path_get_number(ai_path) > 1{  
     path_start(ai_path, 4, 3, 0);  
}  
```  
El código anterior comprueba si "ai_path" tiene más de 1 punto, si es cierto la instancia empezará a moverse a lo largo del path.