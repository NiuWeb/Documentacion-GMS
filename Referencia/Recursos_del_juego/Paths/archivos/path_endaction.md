# path_endaction

Establece u obtiene que debe hacer la instancia al terminar un path.

## Sintaxis

  
```gml  
path_endaction;  
```  

## Argumentos

Ninguno

## Descripción

Con esta variable puede obtener o cambiar la acción de una instancia cuando termina el path actual. Normalmente se establece al momento de iniciar un path con `path_start`, pero es posible cambiarlo a gusto durante el juego. Los valores disponibles son las si[list]guientes constantes:  
  
path_action_stop|Detiene el path|  
---|---|  
path_action_restart|Continua desde la posición inicial, saltando al comienzo del path si no es cerrado|  
path_action_continue|Comienza el path de nuevo desde la posición actual|  
path_action_reverse|Invierte la velocidad del path (recorre el path en reversa)|  

## Devuelve

Constante

## Ejemplo

  
```gml  
if path_endaction == path_action_stop{  
     path_endaction = choose(path_action_restart, path_action_continue, path_action_reverse);  
}  
```  
El código anterior comprueba la acción final del path, si la acción es "detenerse", entonces una nueva acción será seleccionada de forma aleatoria.