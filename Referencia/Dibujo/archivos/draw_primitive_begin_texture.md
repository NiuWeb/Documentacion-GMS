# draw_primitive_begin_texture

Inicia una primitiva con textura de acuerdo al tipo dado.

## Sintaxis

  
```gml  
draw_primitive_begin_texture(kind, texture);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
kind|El tipo de primitiva a iniciar.|  
texture|El índice de la textura a utilizar con la primitiva.|  

## Descripción

Esta función debe ser llamada antes de poder definir cualquier figura primitiva con textura. Se debe indicar el tipo de primitiva a utilizar (ver [`draw_primitive_begin()`](http://docs-gamemaker-es.blogspot.com.co/p/drawprimitivebegin.html) para más información) y la identificación de la textura, la cual puede ser un sprite o background. La identificación de estos recursos pueden obtenerse utilizando las funciones `sprite_get_texture()` y `background_get_texture()` (ingresar -1 en caso de no querer utilizar ninguna textura).  
  
**NOTA:** Para que una textura pueda repetirse, su tamaño debe ser una potencia de dos, por ejemplo: 32x32, 128x128, etc.

## Devuelve

Nada.

## Ejemplo

  
```gml  
tex = background_get_texture(bck_textura);  
len = 64;  
  
draw_set_colour(c_white);  
draw_primitive_begin_texture(pr_trianglefan, tex);  
draw_vertex_texture(len*2, len, 0, 0);  
draw_vertex_texture(len*3, len*2, 1, 0)  
draw_vertex_texture(len*2, len*3, 1, 1);  
draw_vertex_texture(len, len*2, 0, 1);  
draw_primitive_end();  
```  
Imaginando que el background bck_textura existe, y posee la siguiente imagen (de 32x32):  
![](imagenes/draw_primitive_begin_texture2.png)  
El código anterior dibujaría una primitiva cuadrilátera con el siguiente aspecto (con un tamaño total de 128x128):  
![](imagenes/draw_primitive_begin_texture1.png)