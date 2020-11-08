## Cadenas de texto

En muchas ocasiones, es necesario utilizar texto dentro de un juego. Para ello, _GameMaker: Studio_ posee una completa colección de funciones que permiten manupular las cadenas de texto (_cadena de texto_ es otra forma de llamarle a una línea de texto) y modificarlas a necesidad.  
  
Cabe mencionar que existen ciertas convenciones que se pueden utilizar al crear cadenas para incluir determinados caracteres. Por ejemplo, se pueden incluir comillas dobles abriendo la cadena con comillas simples (y viceversa), y se puede forzar un salto de línea (sólo al imprimirse el texto en pantalla) utilizando el caracter _#_; este salto de línea se puede omitir (para mostrar el caracter, y no un salto de línea) escapándolo así: _#_.  

### Relacionados

*   `ansi_char()`
*   `chr()`
*   `is_string()`
*   `ord()`
*   `real()`
*   `string()`
*   `string_char_at()`
*   `string_copy()`
*   `string_count()`
*   `string_delete()`
*   `string_digits()`
*   `string_format()`
*   `string_height()`
*   `string_height_ext()`
*   `string_insert()`
*   `string_length()`
*   `string_letters()`
*   `string_lettersdigits()`
*   `string_lower()`
*   `string_ord_at()`
*   `string_pos()`
*   `string_repeat()`
*   `string_replace()`
*   `string_replace_all()`
*   `string_upper()`
*   `string_width()`
*   `string_width_ext()`

1.  ## Portapapeles
    
    Dentro de la plataforma **Windows**, _GameMaker: Studio_ permite acceder y manipular el portapapeles y su contenido de texto, utilizando las siguientes funciones.  
    
    ### Relacionados
    
    *   `clipboard_get_text()`
    *   `clipboard_has_text()`
    *   `clipboard_set_text()`