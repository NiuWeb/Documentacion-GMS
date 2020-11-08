# keyboard_set_numlock

Establece el estado de la tecla "numberlock".

## Sintaxis

  
```gml  
keyboard_set_numlock(value);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
value|Establece este valor en true para |  

## Descripción

Con esta función puede cambiar la tecla numberlock entre encendido y apagado (**true** para encendido y **false** para apagado)  
  
_**Nota:** Esta funcionalidad solo esta disponible en Windows y esta no funciona en ningún otro dispositivo._

## Devuelve

Nada

## Ejemplo

  
```gml  
if keyboard_get_numlock(){  
     keyboard_set_numlock(0);  
}  
else{  
     keyboard_set_numlock(1);  
}  
```  
El código anterior comprueba el estado de la tecla numberlock y si está encendida (true) la establece en apagado (false) y viceversa.