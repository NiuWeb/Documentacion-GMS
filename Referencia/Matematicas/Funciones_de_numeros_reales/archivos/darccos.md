# darccos

Devuelve el coseno inverso del número dado, siendo éste expresado en grados.

## Sintaxis

  
```gml  
darccos(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El ángulo (en grados) al cual obtener el coseno inverso.|  

## Descripción

Esta función devuelve el coseno inverso del número dado. Básicamente, si `dcos(a)=b`, entonces `darccos(b)=a`. El valor resultante estará entre 180 y 0.  
  
NOTA: Esta función sólo acepta un número entre -1 y 1. Cualquier número fuera de este rango ocacionará un error.

## Devuelve

Número real.

## Ejemplo

  
```gml  
val = darccos(-1); //Devuelve 180  
```