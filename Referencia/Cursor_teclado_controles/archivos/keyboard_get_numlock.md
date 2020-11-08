# keyboard_get_numlock

Obtiene el estado de la tecla "numberlock" del teclado.

## Sintaxis

  
```gml  
keyboard_get_numlock();  
```  

## Argumentos

Ninguno

## Descripción

Puede usar esta función para saber si el teclado numérico esta bloqueado (true) o no (false).  
  
_**Nota:** Esta funcionalidad solo esta disponible en Windows y esta no funciona en ningún otro dispositivo._

## Devuelve

Boleano

## Ejemplo

  
```gml  
if keyboard_get_numlock(){  
     keyboard_set_numlock(0);  
}  
else{  
     keyboard_set_numlock(1);  
}  
```  
El código anterior obtendrá el estado de la tecla "numberlock" y si está activado (true) será apagado (false) y viceversa.