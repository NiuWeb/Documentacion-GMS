# clipboard_set_text

Almacena el texto dado en el portapapeles.

## Sintaxis

  
```gml  
clipboard_set_text(str);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
str|La cadena a almacenar en el portapapeles.|  

## Descripción

Esta función almacena la cadena dada en el portapapeles. Cabe mencionar que con esta función, el portapapeles es limpiado antes de almacenar la cadena, por lo que al ejecutarse no se conservará el contenido copiado anteriormente en el mismo. Es posible usar esta función para limpiar el portapapeles, utilizando una cadena vacía (`""`).  
  
**NOTA:** Esta función es válida sólo para la plataforma **Windows**.

## Devuelve

Nada

## Ejemplo

  
```gml  
clipboard_set_text("¡Estoy copiado en el portapapeles!");  
```  
Se almacena la cadena `"¡Estoy copiado en el portapapeles!"` dentro del portapapeles.