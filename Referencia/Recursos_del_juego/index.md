## Recursos del juego

En GameMaker: Studio es posible definir varios tipos de recursos de juego, como sprites, sonidos, fuentes y backgrounds, y cada tipo de recurso posee una colección de códigos que permiten modificarle de diferentes formas. Es recomendable tener en cuenta las siguientes notas cuando se deseen utilizar estos códigos:  

*   Preferiblemente evitar borrar recursos que se estén utilizando en la sala actual del juego.
*   Si se cambia algún recurso incluído en el juego por un externo, la función `game_restart()` NO restablecerá dichos recursos a su forma original.
*   Crear recursos durante la ejecución puede producir un aumento enorme de memoria fácilmente. Por ejemplo, si se tiene un sprite de 128x128 con 32 subimágenes, y se crean 36 copias transformadas de éste, se consumiría 36x32x128x128x4 = 72MB de información; una barbaridad. Además de esto, los sprites que se añaden durante la ejecución se guardan en una nueva página de textura, y para utilizarse GameMaker: Studio debe realizar muchos cambios de página (_page swaps_), lo que ralentizaría considerablemente el juego. 
*   Es importante asegurarse de eliminar todos los recursos creados en ejecución que ya no se necesiten, pues de lo contrario podría producirse una fuga de memoria y eventualmente un cierre inserperado del juego.

En general, es mala idea reemplazar sprites incluidos durante la ejecución del juego, y es mejor crear los recursos necesarios al inicio del juego y no de la sala.  

### Relacionados

*   Sprites
*   Backgrounds
*   Audio
*   Fuentes
*   [Paths](Paths/)
*   Líneas de tiempo
*   [Habitaciones](Rooms/)

Además, hay dos funciones que permiten manejar el índice y tipo de cualquier recurso del juego:  

*   `asset_get_index()`
*   `asset_get_type()`