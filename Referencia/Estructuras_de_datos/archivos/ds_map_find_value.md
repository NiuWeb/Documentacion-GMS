

# ds_map_find_value

Busca la llave dada y devuelve su valor asignado.

## Síntaxis

  
```gml  
ds_map_find_value(id, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id del mapa a usar.|  
key|La llave a buscar.|  

## Descripción

Con esta función puede buscar el valor de una llave especificada. Para ello debes de indicar el id del mapa a usar y la llave. _**Nota:** Si no existe la llave especificada la función devolverá `undefined`, por lo que debes de comprobar el valor devuelto con la función `is_undefined()`._

## Devuelve

Número real, Cadena de texto o Indefinido

## Ejemplo

  
```gml  
amount = ds_map_find_value(inventory, "food");  
  
//O usando el accesor de mapas "?":  
amount = inventory[? "food"];  
```  
El código anterior obtiene el valor de la llave "food" y la almacena en la variable "amount".