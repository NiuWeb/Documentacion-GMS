## Manejo de archivos

En algún punto de la creación de un videojuego, será necesario almacenar información externamente y recuperarla posteriormente. Por ejemplo, almacenar datos de inicios de sesión, puntajes o progreso de un juego son elementos que deberían guardarse externamente. Es por ello que _GameMaker: Studio_ ofrece difentes funciones para administrar archivos externos.  
  
Algo **muy importante** a tener en cuenta es que _GameMaker: Studio_ está bajo límites de **Sandbox**, lo que significa que posee una serie de limitaciones en cuanto al manejo de archivos, aunque estas limitaciones pueden variar un poco dependiendo de la plataforma.  
[Ver **Anexo: Límites del sistema de archivos**.](archivos/Anexo_limites_sistema_archivos.html)  

1.  ## Sistemas de archivos
    
    Información detallada sobre cada sistema de archivos a continuación:  
    
    ### Relacionados
    
    *   [Funciones generales del sistemas de archivos.](Funciones_generales/index.html)
    *   [Archivos INI.](Archivos_INI/index.html)
    *   [Archivos de texto.](Archivos_de_texto/index.html)
    *   Archivos binarios.
2.  ## Directorios
    
    Obviamente, habrán momentos en los que sea necesario modificar o manejar de algún modo los directorios en los que almacenar los archivos. Para ello, GameMaker: Studio posee una lista de funciones especializadas en directorios:  
    
    ### Relacionados
    
    *   `directory_exists()`
    *   `directory_create()`
    *   `directory_destroy()`
    *   `temp_directory`
    *   `working_directory`
    *   `program_directory`
3.  ## Codificación y cifrado
    
    Cuando se manejan archivos externos, existe la posibilidad de que el usuario pueda abrirlos y modificar la información para alterar los datos del juego. Por esta razón, GameMaker: Studio provee funciones de cifrado y codificación básicas para proteger la información del juego.
    
    ### Relacionados
    
    *   `base64_encode()`
    *   `base64_decode()`
    *   `json_encode()`
    *   `json_decode()`
    *   `md5_string_utf8()`
    *   `md5_string_unicode()`
    *   `md5_file()`
    *   `sha1_string_utf8()`
    *   `sha1_string_unicode()`
    *   `sha1_file()`