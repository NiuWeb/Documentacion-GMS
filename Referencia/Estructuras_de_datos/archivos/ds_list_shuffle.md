# ds_list_shuffle

Mueve a posiciones aleatorias los valores almacenados en una lista.

## Sintaxis

  
```gml  
ds_list_shuffle(id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
id|El id de la lista a desordenar.|  

## Descripción

Con es función puede desordenar una lista, esto moverá todos los valores a posiciones aleatorias dentro de la lista.  
  
_**Nota:** Esta función cambiará los elementos de la lista a las mismas posiciones cada vez que se ejecute nuevamente el juego, debido a que GameMaker:Studio genera la misma semilla al empezar el juego, con el objetivo de que la depuración del código sea más sencilla. Para evitar este comportamiento debe usar la función `randomize()` al inicio del juego. Esto solo es valido mientras se prueba y depura el código del juego, el ejecutable final siempre cambiara la semilla cada vez que se ejecute._

## Devuelve

Nada

## Ejemplo

  
```gml  
if restart{  
     ds_list_shuffle(card_list);  
}  
```  
El código anterior desordena la lista indexada en la variable "card_list" si la variable "restart" es `true`.