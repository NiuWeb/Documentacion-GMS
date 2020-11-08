# room_exists

Devuelve si existe o no una _room_ con el índice dado.

## Sintaxis

  
```gml  
room_exists(índice);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
índice|El índice de la _room_ para comprobar.|  

## Descripción

Con esta función podemos comprobar y ver si la habitación que especifique existe o no. Esta función toma el índice de la _room_ (un número real) y no el nombre de la habitación (una cadena). Esta función es muy útil cuando se están creando _rooms_ dinámicamente usando la función `room_add()`, pero también se puenden usar las variables de lectura `room_first` y `room_last` o las funciones `room_next()` y `room_previous()` para obtener un índice de la habitación específico o proporcionar una variable que ha almacenado el índice de cualquier otra habitación en tu juego.

## Devuelve

Booleano

## Ejemplo

  
```gml  
if room_exists(global.rm[0])  
{  
    room_goto(global.rm[0]);  
}  
```  
El código anterior comprueba si la _room_ indexada en el _array_ `global.rm[]` existe y si es así, entonces va a esa _room_.