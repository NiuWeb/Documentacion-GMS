## Funciones de números reales

Los números reales, en _GameMaker: Studio_, se consideran números de doble precisión con punto flotante. Esto significa que los números no poseen una cantidad fija de cifras decimales o enteras. Por ejemplo, el número 2 es un número entero, pero 2.0 es un número real de punto flotante. Esta distinción entre enteros y flotantes es muy importante cuando se trabaja con multi-plataforma, pues la precisión de los cálculos realizados en una computadora puede no ser la misma que la de un dispositivo móvil. Por ello, debe tenerse especial cuidado cuando se hacen comparaciones numéricas. Por ejemplo:  
  
```gml  
if(image_index == 1)  
{  
    //Hacer algo...  
}  
  
```  
En teoría, **esto funciona**. Pero debido a la forma en la que los puntos flotantes trabajan, es posible que el valor **real** de `image_index` sea de 1.00000000001 y no 1, caso en el que la comparación nunca será verdadera. Este tipo de errores pueden ser un tanto difíciles de depurar, por lo que es bueno ser consciente de estas posibilidades y tomar medidas de aproximación adecuadas para realizar las comparaciones, utilizando funciones de aproximación. Por ejemplo, el anterior código podría escribirse así:  
  
```gml  
if(floor(image_index) == 1)  
{  
    //Hacer algo...  
}  
  
```  
  
**NOTA:** En las plataformas _YoYo Compiler_ (aquellas con las siglas YYC), las expresiones y funciones son evaluadas de izquierda a derecha, mientras que en todas las demás plataformas, éstas son evaluadas de derecha a izquierda, lo que significa que el siguiente código:  
  
```gml  
val = max(num, ++num, num++);  
```  
Devolverá valores distintos dependiendo de la plataforma.  

1.  ## Épsilon de la máquina
    
    El denominado _épsilon_ (**ε**) o _épsilon_ de la máquina es el menor número que se encuentra dentro del margen de aproximación, lo que significa que la computadora evaluará _1.0 + ε > 1,0_ como verdadero. _GameMaker: Studio_ permite manejar la precisión de las aproximaciones modificando el épsilon del juego, utilizando las siguientes funciones.
    
    ### Relacionados
    
    *   `math_set_epsilon()`
    *   `math_get_epsilon()`
2.  ## Funciones de aleatoriedad
    
    _GameMaker: Studio_ posee una serie de funciones que permiten obtener números aleatorios.
    
    ### Relacionados
    
    *   `choose()`
    *   `random()`
    *   `random_range()`
    *   `irandom()`
    *   `irandom_range()`
    *   `random_set_seed()`
    *   `random_get_seed()`
    *   `random_use_old_version()`
    *   `randomize()`
    
      
    **NOTA:** Cuando se utilizan funciones de aleatoriedad, _GameMaker: Studio_ mantiene la misma semilla de aleatoriedad cuando inicia el juego, con el fin de faciltar la depuración. Esto significa que cada vez que se ejecuta el juego, estas funciones devolverán siempre la misma secuencia de números en el mismo orden. Para generar una semilla aleatoria debe usarse la función `randomize()`, o bien puede establecerse una manualmente usando `random_set_seed()`.
3.  ## Funciones trigonométricas
    
    En los videojuegos,suele llegar un punto en el que es indispensable el uso de la trigonometría para desarrollar diferentes mecánicas y operaciones. Por ello, _GameMaker: Studio_ posee una colección de diferentes funciones trigonométricas.
    
    ### Relacionados
    
    *   `arccos()`
    *   `arcsin()`
    *   `arctan()`
    *   `arctan2()`
    *   `sin()`
    *   `tan()`
    *   `cos()`
    *   `darccos()`
    *   `darcsin()`
    *   `darctan()`
    *   `darctan2()`
    *   `dsin()`
    *   `dtan()`
    *   `dcos()`
    *   `degtorad()`
    *   `radtodeg()`
    *   `lengthdir_x()`
    *   `lengthdir_y()`
    
      
    **NOTA:** Cabe mencionar que, en _GameMaker: Studio_, el origen del plano se encuentra en la ezquina superior izquierda de la ventana, lo que significa que en el eje y, el incremento se dirige hacia abajo, y el decremento, hacia arriba. Por ejemplo, un punto (32, 32) se dibujará por encima de un punto (32, 64). Esto debe tenerse en cuenta al trabajar con las funciones trigonométricas.
4.  ## Funciones de aproximación
    
    Funciones para seleccionar o aproximar valores numéricos.
    
    ### Relacionados
    
    *   `round()`
    *   `floor()`
    *   `frac()`
    *   `abs()`
    *   `sign()`
    *   `ceil()`
    *   `max()`
    *   `mean()`
    *   `median()`
    *   `min()`
    *   `lerp()`
    *   `clamp()`
5.  ## Otras funciones
    
    Las funciones matemáticas básicas.
    
    ### Relacionadas
    
    *   `exp()`
    *   `ln()`
    *   `power()`
    *   `sqr()`
    *   `sqrt()`
    *   `log2()`
    *   `log10()`
    *   `logn()`
    *   `int64()`
    *   `is_real()`