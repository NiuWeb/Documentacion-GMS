# dot_product_3d

Devuelve el producto punto de dos vectores

## Síntaxis

  
```gml  
dot_product_3d(x1, y1, z1, x2, y2, z2);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|El componente horizontal del primer vector.|  
y1|El componente vertical del primer vector.|  
z1|El componente z (profundiad) del primer vector.|  
x2|El componente horizontal del segundo vector.|  
y2|El componente vertical del segundo vector.|  
z2|El componente z (profundiad) del segundo vector.|  

## Descripción

Esta función es muy similar a `dot_product()`, con la diferencia de que realiza el cálculo con tres dimensiones:  
  
```gml  
A · B = (Ax * Bx) + (Ay * By) + (Az * Bz)  
  
```  

## Devuelve

Número real.

## Ejemplo

  
```gml  
var x1, y1, x2, y2;  
//Las coordenadas 3d del primer vector  
x1 = 0;  
y1 = 1;  
z1 = 0;  
  
//Las coordenadas 3d del segundo vector.  
x2 = o_Player.x - x;  
y2 = o_Player.y - y;  
z2 = o_Player.z - z;  
  
var dot = dot_product_3d(x1, y1, z1, x2, y2, z2);  
if(dot > 0)  
    above = true;  
else  
    above = false;  
  
```  
En el código anterior, se obtiene el producto punto de los vectores formados por (x1, y1, z1) y (x2, y2, z2). Luego, se comprueba si este valor es mayor a 0, y si es así, establece la variable above a `true`, de lo contrario, le da el valor de `false`.