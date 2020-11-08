# draw_vertex_texture

Define un vértice para una primitiva con textura.

## Sintaxis

  
```gml  
draw_vertex_texture(x, y, xtex, ytex);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
x|La posición horizontal en donde definir el vértice.|  
y|La posición vertical en donde definir el vértice.|  
xtex|La posición horizontal del punto de la textura a utilizar.|  
ytex|La posición vertical del punto de la textura a utilizar.|  

## Descripción

Esta función permite definir la posición de un vértice en una primitiva texturizada. La apariencia final de la primitiva depende del tipo de primitiva escogido (ver [`draw_primitive_begin()`](topic.php?draw_primitive_begin) para más información), el orden de inserción de los vértices y la posición del punto inicial definido en la textura. Para finalizar el proceso y dibujar la primitiva, es necesario utilizar la función `draw_primitive_end()`.  
  
Es posible elegir la parte de la textura a dibujar sobre la superficie de la primitiva configurando adecuadamente las posiciones xtex y ytex (estas coordendas son conocidas como los puntos UV). Estos puntos son definidos con un valor entre 0 y 1, donde la esquina superior izquierda de la textura equivale al punto (0, 0), y la esquina inferior derecha de la misma equivale al punto (1, 1). De esta forma es posible texturizar una primitiva con sólo partes de la imagen definida como textura.  
  
Cuando se dibuja una primitiva texturizada, la textura es mezclada con el color de dibujo definido por `draw_set_colour()`, lo que significa que para dibujar la textura sin mezclar sus colores se debe definir el color de dibujo a blanco (`c_white`), como es mostrado en el ejemplo más adelante.  
  
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