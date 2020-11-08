# sign

Devuelve el signo de un número.

## Sintaxis

  
```gml  
sign(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número a obtener el signo.|  

## Descripción

Esta función devuelve el signo de un número. Es decir, si el número es positivo, devolverá 1; si es negativo, devolverá -1, y si es 0, devolverá 0.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = 3;  
b = 2;  
c = 1;  
  
sa = sign(a); //Devuelve 1  
sx = sign(b - a*2); //Devuelve -1  
sp = sign(c - c); //Devuelve 0.  
```