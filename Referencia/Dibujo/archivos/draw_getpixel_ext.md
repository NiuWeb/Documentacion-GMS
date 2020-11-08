# draw_getpixel_ext

Devuelve el valor completo de color del pixel mostrado en un punto de la pantalla

## Síntaxis

draw_getpixel_ext(x, y);

## Aargumentos

Argumento|Descripción|  
---|---|  
x|La coordenada horizontal del punto a revisar|  
y|La coordenada vertical del punto a revisar|  

## Descripción

Esta función permite obtener el valor de color (ver [Anexo: Manejo de colores](Anexo_manejo_de_colores.html)) de cualquier pixel que se esté dibujando en la actual superficie objetivo de renderizado (por defecto es `application_surface`). Esto significa que los resultados dependen del evento en el que esta función sea llamada, al igual que la superficie que se esté usando actualmente como objetivo de renderizado.  
  
Cabe mencionar que esta función no obtiene valores de opacidad, para eso debes usar `draw_getpixel_ext()`.  
  
**NOTA:** Esta función es extremadamente lenta, y debería ser usada SOLO cuando sea absolutamente necesario.

## Devuelve

Entero

## Ejemplo

  
```gml  
var col = draw_getpixel(32, 128);  
alpha = (col >> 24) & 255  
blue = (col >> 16) & 255  
green = (col >> 8) & 255  
red = col & 255  
```  
Se obtiene el color actualen una posición determinada de la pantalla, y se obtienen sus componentes, incluyendo la opacidad.