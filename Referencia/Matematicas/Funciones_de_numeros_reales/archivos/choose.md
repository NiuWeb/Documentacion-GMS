# choose

Devuelve aleatoriamente uno de los valores dados.

## Sintaxis

  
```gml  
choose(val1, ..., val16);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val1, ..., val16|La serie de valores a escoger. Puede ser cualquier tipo de dato (cadena, real, constante, array, etc.)|  

## Descripción

En ocaciones puede llegar a ser necesario obtener aleatoriamente valores diferentes a números, u obtener números que no se encuentran dentro del orden real o algún rango. En estos casos, la función `choose()` es una mejor alternativa para generar un resultado aleatorio.  
  
**NOTA:** Esta función generará los mismos resultados (en el mismo orden) cada vez que se ejecuta el juego. Esto gracias a que Game Maker Studio genera la misma semilla aleatoria inicial. Para evitar esto, usar `randomize()` al inicio del juego para generar una nueva semilla aleatoria.

## Devuelve

Uno de los argumentos dados.

## Ejemplo

  
```gml  
a[3] = 0;  
b = choose("Una cadena", 32, c_white, a);  
```  
Se le asignará a la variable `b` un valor aleatoriamente. Puede generarse una cadena, un número real, una constante (aunque en realidad también es un número real) o un _array_.