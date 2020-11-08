# ds_grid_create

Crea una nueva grid.

## Sintaxis

  
```gml  
ds_grid_create(w, h);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
w|El ancho de la grid a crear.|  
h|El alto de la grid a crear.|  

## Descripción

Con esta función puede crear una nueva estructura de datos del tipo grid con el especifico número de celdas hacia lo ancho y alto. Esta función devuelve un ID el cual debe de ser almacenado para trabajar con la grid en el futuro.

## Devuelve

Número real

## Ejemplo

  
```gml  
mygrid = ds_grid_create(10, 10);  
```  
El código anterior crea una grid con 10 celdas hacia lo alto y 10 celdas hacia lo ancho.