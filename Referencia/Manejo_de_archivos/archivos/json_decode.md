# json_decode

Decodifica una cadena de objeto JSON en un mapa.

## Sintaxis

  
```gml  
json_decode(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena JSON a decodificar.|  

## Descripción

JSON (JavaScript Object Notation) es un formato ligero de intercambio de datos, el cual es fácil de leer y escribir tanto para personas como para computadoras. Este formato está compuesto de dos estructuras básicas:  

*   Colecciones de parejas nombre:valor, conocidas comúnmente como _diccionarios_ u _objetos_. Con esta función, _Game Maker Studio_ decodifica estos elementos en mapas.
*   Listas de valores, conocidas comunmente como _arrays_ o _secuencias_. Con esta función, _Game Maker Studio_ decodifica estos elementos en listas.

Esta función decodifica una cadena en formato JSON y la convierte en un mapa (ds_map). Si el JSON a ser decodificado requiere una jeraquía de listas y mapas dentro del mapa central, éstos también son decodificados utiliazando las siguientes reglas:  

*   Si el JSON contiene un único valor, se devuelve un mapa con una única llave llamada `"default"`, en donde se encuentra el valor.
*   Si el JSON es una lista o _array_ de valores, se devuelve una mapa con una única llave llamada `"default"`, y dentro de ésta, una lista que contiene los valores.
*   Si el JSON es un objeto o diccionario, se devuelve un mapa con la información.

**NOTA:** Cuando se decodifican arrays o listas de valores, el mapa con la llave "default" es creado **sólo** cuando el array está en el nivel más alto de la estructura. Los arrays que se encuentran dentro de la estructura se decodifican directamente en una lista, sin ésta ser almacenada dentro de un mapa.

## Devuelve

Mapa, o -1 si ocurre un error.

## Ejemplo

  
```gml  
JSON =  
'{  
"Nivel":5,  
"Nombre": "Juan",  
"Puntos": {  
    "Nivel 1": 65,  
    "Nivel 2": 13,  
    "Nivel 3": 0  
},  
"Texto personal": "Soy un usuario de este juego!"  
}';  
  
info = json_decode(JSON);  
nivel = info[?"Nivel"]; //Devuelve 5  
nombre = info[?"Nombre"]; //Devuelve 'Juan'  
puntos = info[? "puntos"]; //Devuelve un mapa  
puntos_Nivel2 = puntos[? "Nivel 2"]; //Devuelve 13  
texto = info[?"Texto personal"]; //Devuelve 'Soy un usuario de este juego!'  
```