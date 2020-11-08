# ds_list_read

Lee una estructura de datos de tipo lista desde una cadena de texto.

## Sintaxis

  
```gml  
ds_list_read(id, str, [legacy]);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista que leerá información.|  
str|La cadena de texto a leer.|  
legacy (optional)|Puede ser true o false, u omitirse.|  

## Descripción

Con esta función puede cargar una lista(ds_list) guardada (que fue escrita previamente como una cadena de texto usando `ds_list_write()`). Primero debe de crear una nueva lista(ds_list) para leer la cadena de texto; si la lista ya existe y contiene información, dicha información será borrada. Esta función es muy importante al crear sistemas de guardado para su juego. Tenga en cuenta que si la lista(ds_list) fue creada con versiones anteriores de GameMaker debería de agregar el argumento opciones "legacy", estableciéndolo como `true`; debido a que el formato fue cambiado en esta versión.

## Devuelve

Nada

## Ejemplo

  
```gml  
list = ds_list_create();  
ini_open("save.ini");  
var str = ini_read_string("Lists", "0", "");  
if str != ""{  
     ds_list_read(list, str);  
}  
ini_close();  
```  
El código anterior crea una lista y almacena su indice dentro de la variable "list". Luego abre el archivo ini y lee una cadena de texto, comprobando primero si no es devuelta una cadena de texto vacía. Si no es una cadena de texto vacía, se lee la lista(ds_list).