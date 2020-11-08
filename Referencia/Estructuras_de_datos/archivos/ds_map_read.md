

# ds_map_read

Lee un mapa de una cadena de texto dada.

## Síntaxis

  
```gml  
ds_map_read(id, str [, legacy]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El índice del mapa donde se guardarán los datos|  
str|La cadena de texto a leer|  
legacy (opcional)|Puede establecerse como true, false u omitirse|  

## Descripción

Esta función toma una cadena de texto previamente creada con la función [ds_map_write](./ds_map_write.html) y la introduce dentro de un mapa previamente creado. SI la mapa a usar para guardar la información de la cadena de texto ya tiene información, esta será eliminada antes de continuar. _Nota: si la estructura de datos fue creada con una versión anterior de GameMaker deberá colocar el argumento "legacy" como `true` debido al cambio de formato en las versiones._

## Devuelve

Nada

## Ejemplo

  
```gml  
inventory = ds_map_create();  
ini_open("map.ini");  
var t_string = ini_read_string("Saved", "0", "");  
if t_string != ""{  
    ds_map_read(inventory, t_string);  
}  
ini_close();  
```  
El codigo anterior crea un nuevo mapa y guarda su índice en la variable "inventory", luego apertura el archivo "map.ini" y almacena dentro de una variable temporal llamada "t_string" una cadena de texto del archivo. Luego comprueba si la cadena de texto no esta vacía, si es así, esta es leída y convertida para ser almacenada dentro del mapa previamente creado.