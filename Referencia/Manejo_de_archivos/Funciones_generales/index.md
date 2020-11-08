## Funciones del sistemas de archivos

Esta sección presenta una lista de las funciones que permiten un manejo global de los archivos externos.  
  
Las siguientes funciones permiten administrar los diferentes archivos:  

*   `file_exists()`
*   `file_delete()`
*   `file_rename()`
*   `file_copy()`
*   `file_find_first()`
*   `file_find_next()`
*   `file_find_close()`
*   `file_attributes()`

  
Las siguientes funciones permiten obtener el nombre de los archivos:  
  
_**NOTA:** Las siguientes funciones **no modifican** el nombre de los archivos reales, sólo trabaja con cadenas de texto._  

*   `filename_name()`
*   `filename_path()`
*   `filename_dir()`
*   `filename_drive()`
*   `filename_ext()`
*   `filename_change_ext()`

  
Finalmente, una serie de funciones especiales exclusivas de la plataforma **Windows** que permiten leer y modificar archivos fuera del _sandbox_ mediante la intervención explícita del usuario:  

*   `get_open_filename()`
*   `get_open_filename_ext()`
*   `get_save_filename()`
*   `get_save_filename_ext()`