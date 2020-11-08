# darcsin

Devuelve el seno inverso del número dado, siendo éste expresado en grados.

## Sintaxis

  
```gml  
darcsin(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El ángulo (en grados) al cual obtener el seno inverso.|  

## Descripción

Esta función devuelve el seno inverso del número dado. Básicamente, si `dsin(a)=b`, entonces `darcsin(b)=a`. El número resultante estará entre -90 y 90.  
  
NOTA: Esta función sólo puede aceptar un número entre -1 y 1. Cualquier número fuera de este rango ocacionará un error.

## Devuelve

Número real.

## Ejemplo

  
```gml  
val = darcsin(-1); //Devuelve -90  
```