# ds_stack_copy

Copia el contenido de una Pila en otra

## Síntaxis

  
```gml  
ds_stack_copy(ds, source);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ds|El id de la nueva Pila.|  
soruce|El id de la Pila a copiar.|  

## Descripción

Esta función puede ser usada para copiar el contenido de una pila dentro de otra. Esto **no** remueve el contenido de la pila original, ni tampoco la destruye. Al usar esta función los valores son copiados dentro de otra pila creada previamente. Si la pila indicada como destino contiene valores, los valores son removidos (por lo tanto se pierde toda la información almacenada).

## Devuelve

Nada

## Ejemplo

  
```gml  
with (instance_create(x, y, obj_Enemy)) {  
     stack = ds_stack_create();  
     ds_stack_copy(stack, other.stack);  
}  
```  
El código anterior crea una nueva instancia y luego de ser creada, crea una nueva pila (ds_stack) y copia el contenido de la pila de la instancia que esta ejecutando el código, dentro de la pila recientemente creada.