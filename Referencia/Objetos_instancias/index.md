# Objetos e instancias

Para crear un juego en _GameMaker: Studio_, es necesario definir **objetos** y añadirlos al _árbol de recursos_. Un objeto puede contener diferentes eventos, en los cuales se puede utilizar tanto piezas de códigos GML como acciones DnD para definir el comportamiento de dicho objeto. Sin embargo, este objeto no está _posicionado_ **dentro** del juego, sólamente actúa como una _plantilla_ para las **instancias**, quienes son las que realmente estarán en las habitaciones. Una instancia, básicamente, es una **copia** del objeto posicionada en una habitación y, debido a esto, puedes crear un solo objeto y posicionar cien instancias de sí mismo en una _room_ para crear el juego.  
  
Otro aspecto a entender acerca de los objetos y las instancias es que, una vez una instancia es creada (en una habitación), ésta puede ser manipulada de forma independiente (usando acciones DnD o códigos GML) sin –necesariamente– tener que recurrir a afectar a las demás instancias del mismo objeto. Por ejemplo, es posible usar el [Menú de instancias](javascript:void(0) "Enlace aún no disponible") del editor de _rooms_ para modificar una instancia única; por ejemplo, para modificar su escala u orientación **sin** afectar a las demás.  
  
Información acerca de las instancias y los objetos en las siguientes páginas:

*   [Objetos](Objetos/)
*   [Instancias](Instancias/)