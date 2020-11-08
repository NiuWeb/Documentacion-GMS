# surface_save

Guarda una surface en el disco.

## Sintaxis

  
```gml  
surface_save(surface_id, fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a guardar.|  
fname|El nombre de la imagen a guardar.|  

## Descripción

Esta función puede guardar una surface en el disco usando el nombre de archivo dado. La surface se debe guardar como un archivo de formato *.png.

## Devuelve

Nada

## Ejemplo

  
```gml  
if keyboard_check_pressed(ord("S"){  
     surface_save(surf, "test.png");  
}  
```  
El código anterior comprueba si la tecla "S" es presionada, si es así, guarda la surface indexada en la variable "surf" en el disco con el nombre de "test.png".