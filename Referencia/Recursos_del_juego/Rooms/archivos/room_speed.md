# room_speed

La velocidad de la _room_ actual en _steps_.

## Sintaxis

  
```gml  
room_speed;  
```  

## Descripción

Esta variable contiene la velocidad de la _room_ actual. Tenga en cuenta que esto **NO** son los FPS (frames por segundo) sino que es el número de _steps_ de juego que GameMaker: Studio intentará manener cada segundo.

## Devuelve

Número Real

## Ejemplo

  
```gml  
alarm[0] = room_speed * 10;  
```  
El código anterior usa room_speed para configurar una alarma para que se ejecute en 10 segundos. El uso de la variable de esta manera se asegurará de que la alarma se ejecute en 10 segundos, no importa qué velocidad se establezca para la _room_.