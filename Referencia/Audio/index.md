# Audio

El motor de audio de GMS está basado en el formato .ogg. Se deben cargar los sonidos en el IDE como .wav o .mp3, pero se puede seleccionar **compressed audio** desde la ventana de propiedades de audio y GMS convertirá los sonidos a .ogg (Ogg Vorbis) cuando se compile el juego. De esta forma se puede mantener el tamaño del juego al mínimo asegurando la máxima calidad. Otro beneficio del motor de audio de GMS es que se tiene acceso a audio streaming así como sonido 3D con la posibilidad de colocar "oyentes" (listeners) para todos los sonidos, así como diferentes "emisores" (emitters) para crear efectos de sonido espectaculares.

Para tener compatibilidad con proyectos antiguos, GMS puede utilizar el motor de audio de legado. Sin embargo no se pueden utilizar ambos motores de auido a la vez. Se puede eliegir el motor de audio desde **Global Game Settings - Pestaña General**.

1.  ## Funciones de Audio Básicas
    
    Las siguientes funciones se usan para utilizar audio de la forma más directa posible, evitando el uso de emisores y permitiendo al usuario tocar sonidos y música fácilmente (los sonidos siempre se generan en la posición del "oyente" y por lo tanto no son afectados por cambios en el "oyente").
    
    *   [audio_exists](javascript:void(0))
    *   [audio_get_name](javascript:void(0))
    *   [audio_get_type](javascript:void(0))
    *   [audio_play_sound](javascript:void(0))
    *   [audio_play_sound_at](javascript:void(0))
    *   [audio_pause_sound](javascript:void(0))
    *   [audio_pause_all](javascript:void(0))
    *   [audio_resume_sound](javascript:void(0))
    *   [audio_resume_all](javascript:void(0))
    *   [audio_stop_sound](javascript:void(0))
    *   [audio_stop_all](javascript:void(0))
    *   [audio_is_playing](javascript:void(0))
    *   [audio_is_paused](javascript:void(0))
    *   [audio_create_stream](javascript:void(0))
    *   [sudio_destroy_stream](javascript:void(0))
2.  ## Funciones de Audio Avanzadas
    
    Las siguientes funciones se han diseñado para tener mayour control del motor de audio. Es recomendable tener un buen conocimiento de cómo funciona el motor de audio antes de usar estas funciones.
    
    *   [audio_sound_set_track_position](javascript:void(0))
    *   [audio_sound_get_track_position](javascript:void(0))
    *   [audio_sound_length](javascript:void(0))
    *   [audio_sound_pitch](javascript:void(0))
    *   [audio_sound_get_pitch](javascript:void(0))
    *   [audio_falloff_set_model](javascript:void(0))
    *   [audio_sound_set_gain](javascript:void(0))
    *   [audio_master_gain](javascript:void(0))
    *   [audio_set_master_gain](javascript:void(0))
    *   [audio_get_master_gain](javascript:void(0))
    *   [audio_channel_num](javascript:void(0))
    *   [audio_debug](javascript:void(0))
    
    Temas más avanzados, como establecer oyentes, grabar audio, o sincronizar múltiples piestas de audio, se pueden encontrar en las siguientes sub-secciones
    
    *   [Emisores de Audio](javascript:void(0))
    *   [Oyentes](javascript:void(0))
    *   [Grupos de audio](javascript:void(0))
    *   [Buffers de Audio](javascript:void(0))
    *   [Sincronización de Audio](javascript:void(0))
3.  ## Funciones de Legado
    
    La siguientes sección contiene información sobre el sistema de audio de legado, que permite compatibilidad con proyectos antiguos, y tiene utilidad en juegos HTML5.
    
    *   [Legado](javascript:void(0))
4.  ## Funciones Obsoletas
    
    Algunas funciones obsoletas se diseñaron específicamente para música.
    
    *   [audio_play_music](javascript:void(0))
    *   [audio_pause_music](javascript:void(0))
    *   [audio_resume_music](javascript:void(0))
    *   [audio_stop_music](javascript:void(0))
    *   [audio_music_is_playing](javascript:void(0))
    *   [audio_music_gain](javascript:void(0))