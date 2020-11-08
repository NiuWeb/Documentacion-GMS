# random_use_old_version

Activa el generador de semillas aleatorias obsoleto.

## Síntaxis

  
```gml  
random_use_old_version(active);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
active|Indica si usar el generador obsoleto (true) o no (false)|  

## Descripción

 La generación de números aleatorios en _GameMaker: Studio_ fue mejorada y el anterior generador fue marcado como obsoleto. Si tienes un juego que requiere semillas generadas por el generador antíguo, tendrás que utilizar esta función para desactivar el generador regular y usar el obsoleto.

## Devuelve

Número real.

## Ejemplo

  
```gml  
random_use_old_version(true);  
```  
Se activa el generador obsoleto.