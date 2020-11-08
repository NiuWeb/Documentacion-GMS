# ini_section_delete

Elimina una sección de un archivo ini.

## Sintaxis

  
```gml  
ini_section_delete(section);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ini a eliminar.|  

## Descripción

Esta función permite eliminar una sección del archivo actualmente abierto, incluyendo todas las llaves (y su respectivo valor) asociadas a ella.

## Devuelve

Nada.

## Ejemplo

  
```gml  
ini_open("perfil.ini");  
ini_section_delete("estadisticas");  
ini_close();  
```  
Se abre el archivo perfil.ini y se elimina la sección `"estadisticas"` junto con todas las llaves asociadas a ella. Posteriormente cierra el archivo.