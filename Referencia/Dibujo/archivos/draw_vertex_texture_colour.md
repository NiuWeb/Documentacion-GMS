# draw_vertex_texture_colour

Define un vértice para una primitiva texturizada con el color y opacidad dados.

## Sintaxis

  
```gml  
draw_vertex_texture_colour(x, y, xtex, ytex, col, alpha);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde definir el vértice.|  
y|La posición vertical en donde definir el vértice.|  
xtex|La posición horizontal del punto de la textura a utilizar.|  
ytex|La posición vertical del punto de la textura a utilizar.|  
col|El color con el cual dibujar el vértice.|  
alpha|La opacidad del vértice.|  

## Descripción

Esta función permite definir la posición de un vértice en una primitiva texturizada, utilizando un color y opacidad propios. La apariencia final de la primitiva depende del tipo de primitiva escogido (ver [`draw_primitive_begin()`](http://docs-gamemaker-es.blogspot.com.co/p/drawprimitivebegin.html) para más información), el orden en el cual se añaden los vértices, el punto de la textura a utilizar y el color y opacidad que se han definido (ver [`draw_vertex_texture()`](http://docs-gamemaker-es.blogspot.com/p/drawvertextexture.html) para más información). Para mantener el color original de la textura, utilizar como color el valor de -1 o la constante `c_white`. Para finalizar el proceso y dibujar la primitiva, es necesario utilizar la función `draw_primitive_end()`.  
  
**NOTA:** Para que una textura pueda repetirse, su tamaño debe ser una potencia de dos, por ejemplo: 32x32, 128x128, etc.

## Devuelve

Nada.

## Ejemplo

  
```gml  
tex = background_get_texture(bck_textura);  
len = 64;  
  
draw_set_colour(c_white);  
draw_primitive_begin_texture(pr_trianglefan, tex);  
draw_vertex_texture_colour(len*2, len, 0, 0, c_white, 1);  
draw_vertex_texture_colour(len*3, len*2, 1, 0, c_blue, 1)  
draw_vertex_texture_colour(len*2, len*3, 1, 1, c_green, 1);  
draw_vertex_texture_colour(len, len*2, 0, 1, c_red, 1);  
draw_primitive_end();  
```  
Imaginando que el background bck_textura existe, y posee la siguiente imagen (de 32x32):  
![](imagenes/draw_primitive_begin_texture2.png)  
El código anterior dibujaría una primitiva cuadrilátera con el siguiente aspecto (con un tamaño total de 128x128):  
  
![](imagenes/draw_vertex_texcol.png)