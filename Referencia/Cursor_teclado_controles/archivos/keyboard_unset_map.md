# keyboard_unset_map

Reinicia el mapeado del teclado a su estado inicial.

## Sintaxis

  
```gml  
keyboard_unset_map();  
```  

## Argumentos

Ninguno

## Descripción

Con esta función puedes re-mapear las teclas a su estado inicial, es decir, las teclas toman su propio valor de nuevo.

## Devuelve

Nada

## Ejemplo

  
```gml  
if keyboard_check_pressed(vk_escape){  
     keyboard_unset_map();  
}  
```  
El codigo anterior reinicia todas las teclas a su configuración inicial al presionar la tecla espaciadora.