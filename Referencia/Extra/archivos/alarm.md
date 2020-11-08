# alarm

Activa una alarma de la instancia.

## Sintaxis

  
```gml  
alarm[0 ... 11];  
```  

## Argumentos

Ninguno

## Descripción

Este array unidimensional es usado para activar los eventos de alarma en una instancia. Hay 12 alarmas integradas en cada instancia de un objeto, y cada alarma tiene su proio evento, el cual se ejecutará cuando la misma llegue a 0. Cabe mencionar que la alarma en realidad no se detiene al llegar a 0, sino en el siguiente _step_, cuando llega a -1. Por ello, si se desea deterner la alarma por alguna razón, debe asignarse el valor de -1, y no 0.  
  
Las alarmas son calculadas en _steps_ de juego, por lo que, por ejemplo, asignar el valor de 30 a una alarma la ejecutará dentro de 30 _steps_.  
  
**NOTA:** Un evento de alarma sin acciones no se ejecutará.  
  
También es posible activar una alarma utilizando la función `alarm_set()`.

## Devuelve

Numero real

## Ejemplo

  
```gml  
instance_create(x, y, bullet);  
alarm[0] = room_speed;  
```  
Se crea una instancia del objeto `bullet`, e inmediatamente se activa la alarma 0, que se ejecutará en un segundo.