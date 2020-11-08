## Cursor, teclado y otros controles

1.  ## Eventos de teclado
    
    Para utilizar el teclado, _GameMaker: Studio_ posee una gran variedad de funciones que pueden ser utilizadas para reconocer diferentes estados del teclado, como una tecla presionada o suelta, así como también almacenar las pulsaciones del teclado (como cadena de texto) y limpiar por completo el estado del mismo.  
      
    **_NOTA:_** _Estas funciones están diseñadas únicamente para las plataformas Windows, Mac y Ubuntu._  
      
    Cada tecla del teclado está -normalmente- definida por un número entero, denominado _código ASCII_. Puedes utilizar directamente el código numérico ASCII de las teclas que necesites, y estas funciones trabajarán perfectamente. Sin embargo, puede llegar a ser difícil recordar tantos números y las relaciones que tienen con el teclado, por lo que _GameMaker: Studio_ posee una serie de constantes para las teclas especiales del teclado más usadas, y la función especial `ord()`, quien permite obtener el código ASCII de determinado caracter.  
    [Ver **Anexo: Constantes de teclado**.](archivos/Anexo_constantes_de_teclado.html)  
    
    ### Relacionados
    
    *   `keyboard_check()`
    *   `keyboard_check_direct()`
    *   `keyboard_check_pressed()`
    *   `keyboard_check_released()`
    *   `keyboard_clear()`
    *   `keyboard_get_map()`
    *   `keyboard_get_numlock()`
    *   `keyboard_key`
    *   `keyboard_key_press()`
    *   `keyboard_key_release()`
    *   `keyboard_lastchar`
    *   `keyboard_lastkey`
    *   `keyboard_set_map()`
    *   `keyboard_set_numlock()`
    *   `keyboard_string`
    *   `keyboard_unset_map()`