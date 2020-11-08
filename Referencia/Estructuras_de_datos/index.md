

# Estructuras de datos

En muchas ocasiones, es necesario almacenar información de forma precisa y ordenada. Es posible utilizar arreglos, pero si necesitas realizar operaciones más complicadas con los datos, como buscar determinados elementos o grupos de ellos, tendrías que programar grandes piezas de código que podría llegar a ser ineficiente, difícil y realmente doloroso de escribir.  
  
Para solucionar esto, GameMaker: Studio posee una serie de estructuras de datos que pueden ser manejadas con funciones especializadas. Existen seis tipos de estructuras de datos disponibles (actualmente sólo una traducida), cada una teniendo sus propias utilidades dependiendo del tipo de información que se desee almacenar y la manera en la que se necesite manupular: Pilas, colas, listas, mapas, colas de prioridad y cuadrículas.  
  
En escencia, todas las estructuras de datos trabajan de la misma forma: Se crea la estructura y se almacena su identificador en una variable. Este identificador se utilizará para referenciar la estructura con la que se desean realizar operaciones. Finalmente, después de haberla utilizado por completo, se debe eliminar de la memoria. Puedes utilizar cuantas estructuras de datos necesites al tiempo, y todas las estructuras pueden almacenar tanto números como cadenas de texto.  
  
**NOTA:** Como con todos los recursos dinámicos, las estructuras de datos consumen memoria y deben ser destruídas siempre cuando dejan de ser necesarias, con el fin de prevenir fugas de memoria y posterior ralentización e incluso posible fallo general del juego.  

## Listas

Una lista es una estructura de datos que almacena información secuencialmente, en el orden en el que es añadida; de forma similar a un arreglo unidimensional. Las listas son estructuras de datos muy flexibles que permiten añadir valores en cualquier posición, teniendo también la posibilidad de ordenar o desordenar los elementos.  
  
Cuando se accede a una lista, es necesario utilizar **valores enteros** como posiciones (índices) de la lista. Todos los índices no enteros se aproximarán al menor entero más cercano automáticamente.

### Relacionados

*   `ds_list_create()`
*   `ds_list_destroy()`
*   `ds_list_clear()`
*   `ds_list_empty()`
*   `ds_list_size()`
*   `ds_list_add()`
*   `ds_list_delete()`
*   `ds_list_find_index()`
*   `ds_list_find_value()`
*   `ds_list_insert()`
*   `ds_list_replace()`
*   `ds_list_shuffle()`
*   `ds_list_sort()`
*   `ds_list_copy()`
*   `ds_list_read()`
*   `ds_list_write()`

## Pilas

Una pila es una estructura de datos de la forma _Ultimo en entrar Primero en salir_. Puedes _apilar_ valores en la estructura y tomarlos. El valor añadido más recientemente es el primero en la pila (justo como una pila de monedas, para conseguir las monedas que están abajo, primero debes tomar las que están encima una a una). Las pilas son usadas cuando hay interrupciones en el manejo, o para funciones recursivas, también para la realización de IA rudimentaria en sus juegos.

### Relacionados

*   `ds_stack_create()`
*   `ds_stack_destroy()`
*   `ds_stack_clear()`
*   `ds_stack_size()`
*   `ds_stack_empty()`
*   `ds_stack_copy()`
*   `ds_stack_top()`
*   `ds_stack_pop()`
*   `ds_stack_push()`
*   `ds_stack_read()`
*   `ds_stack_write()`

## Mapas

Un mapa (ds_map) es una estructura de datos que almacena información en forma de pares de llaves con su respectivo valor. La estructura de datos de tipo mapa es muy útil, pues permite almacenar un valor con una clave relacionada. Por ejemplo, un personaje tieene una cantidad de elementos diferentes (claves) y de cada elemento tiene cierta cantidad (valores), 10 pociones, 100 de oro, 1 espada, etc. Los mapas mantienen toda esta información en un solo lugar, y se pueden agregar valores o buscar valores con su clave correspondiente.  
  
Sin embargo, hay dos puntos que debe de recordar: los mapas no almacenan la información en un orden (reconocible y manejable), por lo que, para buscar una clave es necesario recorrer el mapa buscando de una en una (lo cual es muy lento). Tampoco es posible mantener claves iguales o asignarle a una clave dos valores diferentes.  
  
**NOTA:** las funciones han cambiado desde versiones anteriores de GameMaker, por lo que juegos importados pueden no funcionar o comportarse como espera.

### Relacionados

*   [`ds_map_exists()`](ds_map/ds_map_exists.html)
*   [`ds_map_create()`](ds_map/ds_map_create.html)
*   [`ds_map_add()`](ds_map/ds_map_add.html)
*   [`ds_map_clear()`](ds_map/ds_map_clear.html)
*   [`ds_map_copy()`](ds_map/ds_map_copy.html)
*   [`ds_map_replace()`](ds_map/ds_map_replace.html)
*   [`ds_map_delete()`](ds_map/ds_map_delete.html)
*   [`ds_map_empty()`](ds_map/ds_map_empty.html)
*   [`ds_map_size()`](ds_map/ds_map_size.html)
*   [`ds_map_find_first()`](ds_map/ds_map_find_first.html)
*   [`ds_map_find_last()`](ds_map/ds_map_find_last.html)
*   [`ds_map_find_next()`](ds_map/ds_map_find_next.html)
*   [`ds_map_find_previous()`](ds_map/ds_map_find_previous.html)
*   [`ds_map_find_value()`](ds_map/ds_map_find_value.html)
*   [`ds_map_read()`](ds_map/ds_map_read.html)
*   [`ds_map_write()`](ds_map/ds_map_write.html)
*   [`ds_map_destroy()`](ds_map/ds_map_destroy.html)

Para saber si una estructura de datos existe. Puede utilizarse la función `ds_exists()`