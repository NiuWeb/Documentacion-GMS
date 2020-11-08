# room_persistent

Contiene el estado de la marca persistente de la _room_

## Sintaxis

  
```gml  
room_persistent;  
```  

## Descripción

Esta variable se puede usar para obtener y establecer el indicador persistente para la _room_ actual. Si es persistente, en cuyo caso cada vez que salga de la _room_ y vuelva a entrar a la misma _room_ el estado de las instancias dentro de la _room_ se mantendrán. Sin embargo, si no es persistente, cada vez que regrese a la _room_ se restablecerá a su estado inicial. Usted debería considerar que al usar una habitación persistente utiliza una cantidad de memoria considerablemente mayor que una _room_ normal y no se recomienda tener demasiadas _rooms_ persistentes en su juego.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if vidas < 1  
    {  
    room_persistent = false;  
    room_goto(rm_inicio);  
    }  
```  
El código anterior comprueba la variable "vidas" y si es menor que 1, establecerá la persistencia de la _room_ en _false_ y luego cambiará de _room_.