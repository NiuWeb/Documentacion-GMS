## Anexo: Constantes de teclado

La siguiente lista contiene todas las consantes de teclado que pueden ser utilizadas como parámetro para las funciones de teclado.  
  

Constante GML|Descripción|  
---|---|  
vk_nokey|Constante que representa que no se está presionando **ninguna** tecla|  
vk_anykey|Constante que representa que se está presionando **cualquier** tecla.|  
vk_left|Constante que representa la tecla de _flecha_ izquierda.|  
vk_right|Constante que representa la tecla de _flecha_ derecha.|  
vk_up|Constante que representa la tecla de _flecha_ arriba.|  
vk_down|Constante que representa la tecla de _flecha_ abajo.|  
vk_enter|Tecla _enter._|  
vk_escape|Tecla _escape._|  
vk_space|Barra espaciadora.|  
vk_shift|Cualquiera de las teclas _shift_.|  
vk_control|Cualquiera de las teclas _control_.|  
vk_alt|Cualquiera de las teclas _alt_.|  
vk_backspace|Tecla de retroceso.|  
vk_tab|Tecla _tab_.|  
vk_home|Tecla de inicio.|  
vk_end|Tecla de Fin.|  
vk_delete|Tecla de suprimir.|  
vk_insert|Tecla de insertar.|  
vk_pageup|Tecla de avanzar página (Av pág).|  
vk_pagedown|Tecla de retroceder página (Re pág).|  
vk_pause|Tecla de pausa.|  
vk_printscreen|Tecla de imprimir.|  
vk_f1 ... vk_f12|Constantes para las teclas de función F1, F2, etc.|  
vk_numpad0 ... vk_numpad9|Teclas del teclado numérico (de 0 a 9).|  
vk_multiply|Tecla de multiplicación.|  
vk_divide|Tecla de división.|  
vk_add|Tecla de adición.|  
vk_subtract|Tecla de sustracción.|  
vk_decimal|Tecla de punto decimal.|  

  
La siguiente es una lista de constantes de teclado que sólo pueden usarse con la función  
`keyboard_check_direct()`:  
  

Constante GML|Descripción|  
---|---|  
vk_lshift|Tecla _shift_ izquierda.|  
vk_lcontrol|Tecla _control_ izquierda.|  
vk_lalt|Tecla _alt_ izquierda.|  
vk_rshift|Tecla _shift_ derecha.|  
vk_rcontrol|Tecla _control_ derecha.|  
vk_ralt|Tecla _alt_ derecha.|  

  
Algunos ejemplos:  
  
```gml  
if(keyboard_check(vk_f3))  
    show_message("Se ha presionado la tecla F3");  
  
```