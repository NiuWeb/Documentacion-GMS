# path_delete

Elimina el path dado.

## Sintaxis

  
```gml  
path_delete(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a eliminar.|  

## Descripción

Usando esta función puede eliminar un path de la memoria. Si el path ha sido creado dinamicamente usando `path_add`, no se podrá usar la variable que contenía su indice para acceder al path, por que este ya no existe, si el path a sido creado usando el **Path Editor** no podrá acceder a él durante todo el juego, por que lo esta eliminando permanentemente.

## Devuelve

Nada

## Ejemplo

  
```gml  
var t_path;  
t_path = path_add();  
if mp_grid_path(grid, t_path, x, y, obj_Player.x, obj_Player.y, 1){  
     path_assign(mypath, t_path);  
}  
path_delete(t_path);  
```  
Con el código anterior crea un path y almacena su índice en una variable local. Este path es usado para guardar el path generado por la función `mp_grid_path`, que, si logra encontrar un camino hacia el destino, sera copiado al path "mypath". Por ultimo se elimina "t_path".