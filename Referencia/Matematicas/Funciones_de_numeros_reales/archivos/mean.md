# mean

Devuelve el promedio (media) de una serie de números reales dados.

## Sintaxis

  
```gml  
mean(val1, ..., val16);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val1, ..., val15|Los valores a comparar.|  

## Descripción

Esta función devuelve el promedio entre la serie de hasta 16 números reales que se pueden ingresar. Es decir, opera sumando todos los números argumentados y posteriormente divide el resultado entre la cantidad de números ingresados.

## Devuelve

Número real

## Ejemplo

  
```gml  
a = mean(2, 4, 6, 8); //Devuelve 5, porque 2+4+6+8=20, y 20/4=5  
b = mean(1, 3, 1, 2); //Devuelve 1.75, porque 1+3+1+2=7, y 7/4=1.75  
c = mean(2, 7); //Devuelve 4.5, porque 2+7=9, y 9/2=4.5  
d = mean(3, 2, 5, 4, 1, 2.2); //Devuelve 2.86 aproximadamente, porque 3+2+5+4+1+2.2=17.2, y 17.2/2=2.86 aprox.  
```