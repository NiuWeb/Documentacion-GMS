# surface_save_part

Guarda una parte de una surface en el disco.

## Sintaxis

  
```gml  
surface_save_part(surface_id, fname, x, y, width, height);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a guardar.|  
fname|El nombre de la imagen a guardar.|  
x|La posición en x desde donde se guardará la surface.|  
y|La posición en y desde donde se guardará la surface.|  
width|El ancho de la parte a guardar.|  
height|El alto de la parte a guardar.|  

## Descripción

Esta función guarda una parte de una surface en el disco usando el nombre de archivo dado. La surface debe ser guardada con el formato *.png. La posición (x, y) dadas corresponden a las coordenadas locales de la surface, donde (0, 0) es la esquina superior izquierda de la surface.

## Devuelve

Nada

## Ejemplo

  
```gml  
if keyboard_check_pressed(ord("S"){  
     surface_save_part(surf, "test.png", 0, 0, 100, 100);  
}  
```  
El código anterior comprueba si la tecla "S" ha sido presionada, si es así, guarda una parte de la surface indexada en la variable "surf" en el disco.