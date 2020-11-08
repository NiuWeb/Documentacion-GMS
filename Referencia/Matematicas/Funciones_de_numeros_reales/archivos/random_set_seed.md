# random_set_seed

Establece la semilla de la cual los números aleatorios se basarán para generarse.

## Sintaxis

  
```gml  
random_set_seed(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|La nueva semilla.|  

## Descripción

Para generar un número aleatorio, Game Maker Studio toma como base una semilla de aleatoriedad. Con esta función es posible establecer el valor de dicha semilla manualmente para ligar la salida de números aleatorios a una secuencia determinada.

## Devuelve

Nada.

## Ejemplo

  
```gml  
random_set_seed(1);  
```  
Se establece la semilla aleatoria a 1.