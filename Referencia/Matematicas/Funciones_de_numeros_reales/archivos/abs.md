# abs

Obtiene el valor absoluto de un número.

## Sintaxis

  
```gml  
abs(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El número al cual obtener su valor absoluto.|  

## Descripción

Esta función devuelve el número `val` con signo positivo. Es decir que si se argumenta un número positivo, se devolverá el mismo número, pero si se argumenta un número negativo, éste se multiplicará por -1.

## Devuelve

Número real

## Ejemplo

  
```gml  
a = -5; //Devuelve -5  
b = abs(a);//Devuelve 5  
c = 7; //Devuelve 7  
d = abs(c); //Devuelve 7  
e = b - c; //Devuelve -2  
f = abs(e); //Devuelve 2  
```