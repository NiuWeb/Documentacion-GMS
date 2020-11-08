# keyboard_key_press

Simula el presionar la tecla dada.

## Sintaxis

  
```gml  
keyboard_key_press(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|La tecla que se simulará presionar.|  

## Descripción

Con esta función puede simular que se presiona cualquier tecla. Esta función acepta cualquier constante _vk__ y también las teclas estándares del código ASCII.

## Devuelve

Nada

## Ejemplo

  
```gml  
keyboard_key_press(vk_space);  
```  
El código anterior simula el presionar la tecla de espacio.