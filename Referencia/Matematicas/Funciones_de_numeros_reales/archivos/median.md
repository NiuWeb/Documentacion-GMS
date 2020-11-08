# median

Devuelve la mediana (valor intermedio) de un grupo de números reales.

## Sintaxis

  
```gml  
median(val1, ..., val15);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val1, ..., val15|Los valores a comparar.|  

## Descripción

Esta función devuelve la mediana de un grupo dado de números reales. Si la cantidad de números ingresados es **par**, se devolverá el menor número central.

## Devuelve

Número real

## Ejemplo

  
```gml  
a = median(2, 4, 6); //Devuelve 4.  
b = median(3, 1, 2, 5); //Devuelve 2.  
```