# room_previous

Esto devolverá el índice de la _room_ anterior del índice de la _room_ dada.

## Sintaxis

  
```gml  
room_previous(num);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
num|El índice de la sala desde donde comprobar.|  

## Descripción

Con esta función puede obtener el índice de la _room_ anterior del índice dado en el argumento "num". Por ejemplo, puede usar la variable `room` de **sólo lectura** para obtener el índice de la _room_ actual y luego usar esta función para encontrar la _room_ que viene antes en el árbol de recursos. Si no hay _room_ antes de la entrada, se devuelve -1.

## Devuelve

Número Real

## Ejemplo

  
```gml  
if room_previous(room) != -1  
    {  
    room_goto(room_previous(room));  
    }  
```  
El código anterior verificará si la _room_ anterior existe y si es así, irá a ella.