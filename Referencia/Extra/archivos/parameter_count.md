# parameter_count

Devuelve el número de parámetros de línea de comandos.

## Sintaxis

  
```gml  
parameter_count();  
```  

## Argumentos

Ninguno

## Descripción

Los parámetros de línea de comandos son información extra que se puede agregar a un programa cuando se es ejecutado. Con esta función es posible obtener la cantidad de estos parámetros insertador para el juego actual. El primer parámetro tiene como índice el número 1 (El índice 0 es especial: Contiene la ruta completa del ejecutable). Esta función puede ser utilizada en la plataforma HTML5, en donde los parámetros son los datos enviados por URL.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
numero_de_parametros = parameter_count();  
```