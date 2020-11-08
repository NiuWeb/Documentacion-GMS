# path_add_point

Agrega un punto al path dado.

## Sintaxis

  
```gml  
path_add_point(index, x, y, speed);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path al cual se le agregará el punto.|  
x|La coordenada en x del nuevo punto.|  
y|La coordenada en y del nuevo punto.|  
speed|El factor de velocidad del nuevo punto (por defecto es 100).|  

## Descripción

Con esta función puede agregar un punto al path especificado y establecer su factor de velocidad. Este punto es agregado al final del path, sin importar su posición dentro del cuarto, el factor será igual al porcentaje de `path_speed` que la instancia tenga en ese punto del path. Si desea colocar un punto del path en otra posición que no sea el final, debe usar la función `path_insert_point`.

## Devuelve

Nada

## Ejemplo

  
```gml  
path = path_add();  
var i;  
i = 0;  
repeat(10){  
     path_add_point(path, x + lengthdir_x(50, i), y + lengthdir_y(50, i), 100);  
     i += 36;  
}  
```  
El código anterior crea un path circular alrededor de la posición (x, y) de la instancia que ejecuta el código.