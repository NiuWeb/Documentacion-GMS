# ds_stack_read

Lee una pila desde una cadena de texto.

## Síntaxis

  
```gml  
ds_stack_read(ds, str [, legacy] );  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la pila de la que se tomará.|  
str|El texto del cual se leerá.|  
legacy (opcional)|Puede ser true o false u omitirse.|  

## Descripción

Con esta función puede recrear una pila (ds_stack) guardada (la cual ha sido previamente escrita como una cadena de texto usando `ds_stack_write()`. Debe crearse primero una pila(ds_stack) en la cual serpa almacenada la información, si la pila(ds_stack) contiene información, esta información sera removida. Esta función es muy importante cuando se esta creando una mecánica de guardado/carga en su juego.  
  
**NOTA:** Si la estructura de datos fue creada en una versión anterior de _GameMaker_ debe agregar el argumento opcional "legacy", estableciéndolo como true, por que el formato de la cadena de texto a cambiado en esta versión.

## Devuelve

Nada

## Ejemplo

  
```gml  
stack = ds_stack_create();  
ini_open("save.ini");  
var str = ini_read_string("Stacks", "0", "");  
if str != ""{  
     ds_stack_read(stack, str);  
}  
ini_close();  
```  
El código anterior crea una pila y almacena su indice en la variable "stack". Luego abre un archivo ini y lee una cadena de texto de este archivo, comprueba si la cadena de texto no esta vacía primero. Esta cadena de texto es leída por la pila (ds_stack) creada recientemente.