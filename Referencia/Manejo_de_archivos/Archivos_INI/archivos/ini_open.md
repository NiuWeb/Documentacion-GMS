# ini_open

Abre el archivo ini establecido para lectura y escritura.

## Sintaxis

  
```gml  
ini_open(fname);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El nombre del archivo ini a abrir.|  

## Descripción

Esta función permite abrir un archivo ini para lectura y escritura de la información que éste posee. Si el archivo proporcionado no existe, GameMaker: Studio lo creará si se escribe información en él; de lo contrario, las funciones de lectura devolverán el valor por defecto, mas el archivo no será creado.  
  
Cabe mencionar que sólo es posible tener abierto un archivo ini simultáneamente; por ello, es importante utilizar `ini_close()` para cerrar el archivo. Además, la información que se escriba en el archivo no se guardará en el disco duro hasta que esta función sea llamada.  
  

## Devuelve

Nada.

## Ejemplo

  
```gml  
ini_open("datos.ini");  
monedas = ini_read_real("datos", "monedas", 0);  
nivel = ini_read_real("datos", "nivel", 1);  
nombre = ini_read_string("datos", "nombre", "Player");  
ini_close();  
```  
Se abre el archivo datos.ini para lectura y escritura. Posteriormente se leen algunos datos del archivo y por último éste se cierra.