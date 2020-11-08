# random_get_seed

Devuelve la semilla aleatoria actual.

## Sintaxis

  
```gml  
random_get_seed();  
```  

## Argumentos

Ninguno

## Descripción

Para generar un número aleatorio, Game Maker Studio toma como base una semilla de aleatoriedad. Con esta función es posible obtener dicha semilla, la cual puede ser almacenada para reproducir series específicas de eventos aleatorios. Por ejemplo, en un juego se ha producido una serie de números aleatoriamente; entonces, se guarda la semilla con la cual estos números fueron generados para posteriormente cargarla y reproducir la misma serie de números aleatorios.

## Devuelve

Número real.

## Ejemplo

  
```gml  
randomize();  
for(var i = 0; i < 5; i++)  
    numero[i] = irandom(8);  
semilla = random_get_seed();  
```  
Se genera una semilla aleatoria nueva, y luego una serie de 5 números aleatoriamente que se guardan en un _array_. Posteriormente, se guarda en la variable `semilla` la semilla con la que estos números fueron creados, para poderlos volver a generar después.