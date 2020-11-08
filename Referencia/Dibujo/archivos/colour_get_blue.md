# colour_get_blue

Obtiene el componente azul de un color dado

## Sintaxis

  
```gml  
colour_get_blue(col);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
col|El color al cual obtener el componente azul|  

## Descripción

Esta función devuelve la _"cantidad de azul"_ que determinado color. Este componente es un número entero de 0 a 255, donde 0 significa _"sin azul"_ y 255 _"con todo el azul"_. La siguiente imagen ilustra esto:  

![](imagenes/get_blue.png)

## Devuelve

Entero

## Ejemplo

  
```gml  
color = c_teal;  
comp_azul = colour_get_blue(color);  
```  
El código anterior obtendrá el componente azul de la constante de color `c_teal` y lo almacenará en la variable `comp_azul`.