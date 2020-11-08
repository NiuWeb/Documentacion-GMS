# room_goto

Esto se utiliza para ir a una _room_ determinada.

## Sintaxis

  
```gml  
room_goto(num);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
num|El índice de la _room_ a la que ir.|  

## Descripción

Esta función finalizará la _room_ actual e irá a la _room_ especificada en la entrada. La _room_ debe existir, de lo contrario se mostrará un error, y si utiliza la misma _room_ que en la que se encuentra tendrá el mismo efecto que `room_restart`. Tenga en cuenta que la _room_ no cambiará hasta el final del evento en el que se llamó la función, por lo que cualquier código después de que se haya llamado se seguirá ejecutando.

## Devuelve

N/A

## Ejemplo

  
```gml  
switch (global.rm)  
    {  
    case 0: room_goto(rm_level1); break;  
    case 1: room_goto(rm_level2); break;  
    case 2: room_goto(rm_level3); break;  
    }  
```  
El código anterior comprobará una variable global y cambiará de _room_ en función del valor que tenga.