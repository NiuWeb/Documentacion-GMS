# room_get_name

Devuelve el nombre de la _room_ con el índice dado.

## Sintaxis

  
```gml  
room_get_name(índice);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
índice|El índice de la _room_ para comprobar su nombre.|  

## Descripción

Esta función se puede utilizar para devolver el nombre de la _room_ especificada como una cadena. Tenga en cuenta que esto es sólo una cadena y no se puede utilizar para hacer referencia directamente a la _room_. Sin embargo, puede utilizar esta cadena para obtener el índice de la _room_ utilizando la cadena devuelta juento con la función `asset_get_index()`.

## Devuelve

Cadena de Texto

## Ejemplo

  
```gml  
var nombreroom = room_get_name(room);  
draw_text(32, 32, nombreroom);  
```  
El código anterior obtendrá el nombre de la _room_ actual y lo dibujará en la pantalla.