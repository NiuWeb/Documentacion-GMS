# string_width_ext

Devuelve el anchor (en pixeles) de una cadena de texto, basado en la separación entre líneas y anchor máximos dados.

## Sintaxis

  
```gml  
string_width_ext(str, sep, w);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a la cual obtener su anchor.|  
sep|La separación entre líneas, como si la cadena fuera a ser dibjada.|  
w|El anchor máximo, como si la cadena fuera a ser dibjada.|  

## Descripción

Esta función devuelve el anchor (en pixeles) de la cadena ingresada, tomando en cuenta la separación de línea y el anchor máximo de línea (el cual es definido como el número de pixeles que la cadena puede ocupar antes de insertar un salto de línea). El resultado depende de la fuente definida actualmente para dibujo. Tanto la separación como el anchor máximo pueden ser establecidos a -1 para configurar el valor por defecto.

## Devuelve

Número real.

## Ejemplo

  
```gml  
a = "Un texto largo, que en realidad es corto";  
b = string_width_ext(a, 96, 16);  
draw_text_ext(32, 32, a, 96, 16);  
draw_text_ext(32 + b, 32, "Un texto abajo de ese", 96, 16);  
```  
Se dibuja un texto con un anchor máximo de 96px y una separación entre líneas de 16px. Posteriormente se dibuja otro texto con las mismas propiedades justo al frente del anterior.