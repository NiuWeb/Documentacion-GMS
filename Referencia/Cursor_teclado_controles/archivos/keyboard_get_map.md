# keyboard_get_map

Obtiene el código ASCII asignado actualmente a la tecla dada.

## Sintaxis

  
```gml  
keyboard_get_map(key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
key|Esta es la tecla de la que se desea obtener el código ASCII asignado.|  

## Descripción

Es posible que desee obtener el código ASCII que esta asignado actualmente a una tecla (por ejemplo, para saber si está asignada a la tecla que deseamos) lo cual puede ser hecho con esta función.

## Devuelve

Entero

## Ejemplo

  
```gml  
if keyboard_get_map(ord("A")) == ord("A"){  
     keyboard_set_map(ord("A"), keyboard_lastkey);  
}  
```  
En el código anterior comprueba si la tecla _A_ a sido asignada a otra tecla, y si esto no ha sucedido la asigna a la ultima tecla que el usuario a presionado.