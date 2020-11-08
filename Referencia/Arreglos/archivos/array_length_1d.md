# array_length_1d

Devuelve la cantidad de elementos de un _array_ unidimensional.

## Sintaxis

  
```gml  
array_length_1d(arr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
arr|El _array_ a revisar.|  

## Descripción

Con esta función es posible obtener el largor (número de elementos) de un _array_ unidimensional. Para _arrays_ bidimensionales es recomendable el uso de las funciones `array_height_2d()` y `array_length_2d()`.  
  
**NOTA:** Si el _array_ tiene más de 32000 elementos, esta función devolverá resultados erróneos, y no deberá ser usada (en tal caso es más recomendable considerar el uso de listas).

## Devuelve

Número entero.

## Ejemplo

  
```gml  
array[0] = 3;  
array[1] = 5;  
array[2] = 2.2;  
array[3] = 3.2;  
  
len = array_length_1d(array); //Devuelve 4.  
```