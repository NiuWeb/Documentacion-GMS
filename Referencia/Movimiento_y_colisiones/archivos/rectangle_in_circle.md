# rectangle_in_circle

Comprueba si un área rectangular colisiona o se encuentra contenida dentro del área circular dada.

## Sintaxis

  
```gml  
rectangle_in_circle(x1, y1, x2, y2, cx, cy, r);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x1|El componente horizontal del primer punto del área rectangular.|  
y1|El componente vertical del primer punto del área rectangular.|  
x2|El componente horizontal del segundo punto del área rectangular.|  
y2|El componente vertical del segundo punto del área rectangular.|  
cx|La posición horizontal del área circular.|  
cy|La posición vertical del área circular.|  
r|El radio del área circular.|  

## Descripción

Esta función permite comprobar si el área rectangular definida colisiona, completamente o sólo con una parte, con el área circular dada.  
Si el área rectangular no colisiona de ninguna forma con el área circular, la función devolverá 0; si el área rectangular se encuentra completamente dentro del área circular, la función devolverá 1; y si sólo una parte del área rectangular choca con el área circular, la función devolverá 2. En la siguiente imagen se puede apreciar una explicación mejor detallada:  
  
![](https://1.bp.blogspot.com/-UbHgItPw3pg/WcHnJREuJTI/AAAAAAAAAaA/FJlzprNkkMgyBjPajNb0soquxfHeiIB3gCLcBGAs/s1600/rectangle_in_circle.png)

## Devuelve

Número real.