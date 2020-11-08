# is_real

Comprueba si un valor es un número real.

## Sintaxis

  
```gml  
is_real(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El valor a comprobar.|  

## Descripción

Esta función comprueba si una variable almacena un número real (en cuyo caso devolvería `true`) o no (en cuyo caso devolvería `false`).

## Devuelve

Booleano.

## Ejemplo

  
```gml  
a = 5;  
b = "hola";  
c = false;  
  
p = is_real(a); //Devuelve true  
t = is_real(b); //Devuelve false  
k = is_real(c); //Devuelve true  
```