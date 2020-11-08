# Objetos

_GameMaker: Studio_ trae consigo un serie de funciones que permiten obtener detalles acerca de cualquier objeto. Cabe mencionar que un objeto **no es** una instancia, es solamente un recurso base para éstas. Esto significa que los valores obtenidos por estas instancias pueden ser diferentes a los que lleguen a tener las instancias en la habitación durante el juego, pues éstas pueden modificarse individualmente.

### Relacionados

*   `object_exists()`
*   `object_index`
*   `object_get_depth()`
*   `object_get_mask()`
*   `object_get_name()`
*   `object_get_parent()`
*   `object_get_persistent()`
*   `object_get_solid()`
*   `object_get_sprite()`
*   `object_get_visible()`
*   `object_get_physics()`
*   `object_is_ancestor()`

Hay además una serie de funciones que permiten establecer el valor de ciertas propiedades para un objeto. Esto ( por las razones mencionadas anteriormente) puede no afectar a las instancias actualmente existentes en la habitación, pero sí que lo hará con las que se creen posteriormente a la modificación.

### Relacionados

*   `object_set_depth()`
*   `object_set_mask()`
*   `object_set_persistent()`
*   `object_set_solid()`
*   `object_set_sprite()`
*   `object_set_visible()`

Finalmente, es posible usar ciertas funciones para ejecutar eventos dentro de un objecto o instancia específica. Estas funciones pueden ser muy útiles, especialmente cuando se lidia con objetos Padres e hijos.

### Relacionados

*   Generando eventos.