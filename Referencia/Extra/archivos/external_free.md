# external_free

Libera de la memoria las funciones externas asociadas con la _dll_ o _dylib_ dada.

## Sintaxis

  
```gml  
external_free(name);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
name|El nombre de la dll o dylib que desea liberar|  

## Descripción

Esta función libera la memoria asociada con la _dll_ o _dylib_ con el nombre dado. Esto debería hacerse cuando la extensión en cuestión no será necesitada en el juego, como por ejemplo en el evento _game end_.

## Devuelve

Nada

## Ejemplo

  
```gml  
external_free("MyDLL.dll");  
  
```  
El anterior código liberará la memoria relacionada a la extensión _MyDLL.dll_.