# ds_exists

Comprueba si existe una estructura de datos con el tipo dado.

## Síntaxis

  
```gml  
ds_exists(ind, type);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
ind|La variable con el indice a comprobar.|  
type|El tipo de estructura de datos a comprobar (mire la lista de constante debajo).|  

## Descripción

Con esta función puede comprobar si existe una estructura de datos que coincida con el tipo indicado. Usted debe dar el valor "índice" (guardado en una variable) y el "tipo", puede comprobar los tipos en la lista de abajo, la función devuelve `true` si la estructura de datos existe y `false` en caso contrario.  
  

Constante|Descripción|  
---|---|  
ds_type_map|Una estructura de tipo mapa.|  
ds_type_list|Una estructura de tipo lista.|  
ds_type_stack|Una estructura de tipo pila.|  
ds_type_grid|Una estructura de tipo rejilla.|  
ds_type_queue|Una estructura de tipo cola.|  
ds_type_priority|Una estructura de tipo prioridad.|  

## Devuelve

Booleano

## Ejemplo

  
```gml  
if !ds_exists(ai_grid, ds_type_grid){  
     ai_grid = ds_grid_create(room_width / 32, room_height / 32);  
}  
```  
El código anterior comprueba la variable (previamente iniciada) "ai_grid" para comprobar si tiene indexada una rejilla(ds_grid), si no es así, entonces crea una y almacena su índice en la variable.