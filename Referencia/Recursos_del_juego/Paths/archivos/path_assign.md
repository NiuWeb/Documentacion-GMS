# path_assign

Duplica un path existente.

## Sintaxis

  
```gml  
path_assign(index, path);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path en que se escribirá.|  
path|El índice del path que será escrito en 'index'.|  

## Descripción

Con esta función puede copiar los datos de un path a otro path. El path al que se copiará se borrará primero (si tiene datos) y se sobrescribirá con el path que será copiado. Ninguno de los path se eliminan, el resultado son dos paths iguales, pero con índices diferentes.

## Devuelve

Nada

## Ejemplo

  
```gml  
mypath = path_add();  
path_assign(mypath, choose(path_1, path_2, path_3));  
```  
El código anterior crea un nuevo y vació path con el índice en la variable "mypath". Luego copia los datos de uno de las tres posibilidades de path dados.