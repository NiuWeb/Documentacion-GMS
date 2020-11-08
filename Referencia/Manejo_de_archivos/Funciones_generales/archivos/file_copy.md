# file_copy

Copia el archivo dado.

## Sintaxis

  
```gml  
file_copy(fname, newfile);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
fname|El archivo a copiar.|  
newfile|El nuevo archivo.|  

## Descripción

Esta función permite duplicar el archivo especificado, dándole un nuevo nombre. Si se realiza esta acción en Android desde un archivo incluído (el cual se encuentra dentro del APK), el archivo se copiará en la memoria, por lo que copiar archivos grandes puede ocacionar problemas de rendimiento.

## Devuelve

Nada

## Ejemplo

  
```gml  
file_copy("Niveles_incompletos/Nivel07.ini", "Niveles_completos/Nivel07.ini");  
```