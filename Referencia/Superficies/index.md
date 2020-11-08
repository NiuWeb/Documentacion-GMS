## Superficies

En escencia, una superficie (_surface_ en inglés) es un lienzo en donde se podrán dibujar todo tipo de elementos con las funciones de dibujo tradicionales. La ventaja principal que las diferencia es que no se tienen que dibujar todos elementos que la componen en cada fotograma; basta con dibujarlos sobre la superficie una vez (o las que sean necesarias) y después dibujar sólo la superficie completa.  
  
Normalmente, los eventos de dibujo no actúan directamente a la pantalla, sino que dibujan sobre una superficie denominada _application surface_. Esta superficie es, básicamente, un lienzo vacío que puede ser manipulado antes de dibujarse en pantalla, aunque por defecto GameMaker: Studio lo configura automáticamente (aún así, es posible manipular manualmente las propiedades de ésta).  
  
Sin embargo, aparte de la application surface, es posible crear superficies propias y usarlas para crear todo tipo de efectos especiales en el juego. Por ejemplo, puede usarse una superficie para grabar marcas como sangre o escombros sin tener que dibujarlos todos uno por uno, sólo la superficie en general.  
  
Normalmente, las superficies son algo fáciles de utilizar, aunque hay ciertos factores que deben tenerse muy en cuenta a la hora de utilizarlas:  

1.  Primero, es vital entender que las superficies (a exepción de la _application surface_) son "volátiles". Esto significa que si, por ejemplo, el dispositivo o la ventana es minimizada o pierde su _foco_, cualquier superficie puede ser destruida **sin aviso previo**. Esto es a causa de que las superficies se almacenan en la memoria de textura, y ésta puede sobreescribirsecuando la plataforma necesita dicha memoriapara algo más. Es por ello que es importante tener un código de "recuperación" o redibujado, acompañado de la función `surface_exists()`.
2.  Cabe aclarar, además, que las superficies requieren hacer uso de mucha memoria de textura para ser utilizados, por lo que es recomendable mantenerlas tan pequeñas y ligeras como sea posible. Normalmente, es bueno intentar mantenerlas de un tamaño no mayor al de la ventana o vista.
3.  Es recomendable intentar dibujar dentro de las superficies en el evento _Draw_. Esto no es un requerimiento, ni tampoco es posible siempre, pero debido a la manera optimizada en la que _GameMaker: Studio_ dibuja en la pantalla, es recomendable mantener todas las funciones de dibujo dentro de los eventos de dibujo.
4.  Cuando se dibuja una superficie manualmente, ésta se encuentra **siempre** en la posición (0, 0). Esto significa que puedes llegar a tener que convertir coordenadas absolutas (origen de la sala) a coordenadas dentro de las locales de la superficie (origen de la supreficie). Por ejemplo, si se tiene una superficie del tamaño de la vista, y se desea dibujar dentro de ella un elemento que sigue dicha vista, será necesario restarle a las coordenadas de este elemento la posición de la vista, para obtener una posición relativa a la posición (0,0) de la superficie.

### Relacionados

*   `surface_exists()`
*   `surface_create()`
*   `surface_create_ext()`
*   `surface_resize()`
*   `surface_set_target()`
*   `surface_set_target_ext()`
*   `surface_reset_target()`
*   `surface_copy()`
*   `surface_copy_part()`
*   `surface_get_height()`
*   `surface_get_width()`
*   `surface_get_texture()`
*   `surface_getpixel()`
*   `surface_getpixel_ext()`
*   `surface_free()`
*   `surface_save()`
*   `surface_save_part()`