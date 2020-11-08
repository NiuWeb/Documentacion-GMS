# json_encode

Codifica un mapa en una cadena con formato JSON.

## Sintaxis

  
```gml  
json_encode(map);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
map|El mapa a codificar.|  

## Descripción

JSON (JavaScript Object Notation) es un formato ligero de intercambio de datos, el cual es fácil de leer y escribir tanto para personas como para computadoras.  
  
Esta función codifica un mapa previamente creado en una cadena en formato JSON, la cual puede ser útil para, por ejemplo, enviar la información a través de una URL o almacenarla de forma externa, como en un archivo.  
  
NOTA: La funcionalidad jearárquica de JSON está disponible con mapas y listas, por lo que es posible codificar sub-mapas y listas también.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
info = ds_map_create();  
ds_map_add(info, "usuario", "Pedro");  
ds_map_add(info, "puntos", 13);  
ds_map_add(info, "arma", "Lanza");  
  
data = json_encode(info);  
```  
Se codifica la información almacenada en el mapa `info` dentro de la variable `data`, la cual obtendría el siguiente valor:  
  
```gml  
'{ "arma": "Lanza", "puntos": 13.000000, "usuario": "Pedro" }'  
```