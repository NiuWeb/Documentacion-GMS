# ini_key_delete

Elimina una llave de un archivo ini.

## Sintaxis

  
```gml  
ini_key_delete(section, key);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
section|La sección del archivo ni en donde se encuentra la llave a eliminar.|  
key|La llave a eliminar.|  

## Descripción

Con esta función es posible eliminar una llave (y su respectivo valor=) de un archivo ini. La llave a eliminar debe existir.

## Devuelve

Nada.

## Ejemplo

  
```gml  
ini_open("perfil.ini");  
ini_key_delete("perfil", "nivel");  
ini_close();  
```  
Se abre el archivo perfil.ini y se elimina la llave `"nivel"` de la sección `"perfil"`. Posteriormente se cierra el archivo.