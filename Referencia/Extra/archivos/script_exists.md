# script_exists

Comprueba si el script con el índice dado existe.

## Sintaxis

  
```gml  
script_exists(scr);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
scr|El índice del _script_ a comprobar.|  

## Descripción

Esta función comprueba si existe un _script_ con el índice dado (en cuyo caso devuelve `true`) o no (en cuyo caso devuelve `false`). Este índice no es una cadena, sino el nombre del recurso del _script_ (como aparece escrito en el IDE).

## Devuelve

Booleano

## Ejemplo

  
```gml  
scripts[0] = scr_mover_derecha;  
scripts[1] = -1;  
scripts[2] = scr_mover_izquierda;  
  
action = irandom(2);  
  
if(script_exists(scripts[action]))  
    script_execute(scripts[action]);  
```  
Se crea un _array_ de 3 índices; en dos de ellos contiene el índice de un script, y en el tercero, -1. Posteriormente, se obtiene un valor aleatorio de dicho _array_, y si este valor es un script, se ejecuta.