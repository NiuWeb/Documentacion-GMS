# keyboard_key_release

Simula el soltar la tecla dada.

## Sintaxis

  
```gml  
keyboard_key_release(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla que se simulará soltar.|  

## Descripción

Con esta función puede simular soltar cualquier tecla. Esta función acepta cualquier constante **vk_** y también cualquier tecla del estándar del código ASCII.

## Devuelve

Boleano

## Ejemplo

  
```gml  
keyboard_key_release(vk_space);  
```  
Con este código simula que soltar la tecla espacio.