# path_get_kind

Devuelve si el path es "suavizado" o "recto".

## Sintaxis

  
```gml  
path_get_kind(index);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
index|El índice del path a comprobar.|  

## Descripción

Los paths pueden ser suavizados o rectos (un path liso calcula una trayectoria con curvas entre los puntos del path; un path recto va de punto a punto). Esta función devuelve si el path es suavizado (true) o no (false).

## Devuelve

Boleano

## Ejemplo

  
```gml  
kind = path_get_kind(c_path);  
```  
Se establece "kind" en `true` o `false` dependiendo del valor establecido de "c_path".