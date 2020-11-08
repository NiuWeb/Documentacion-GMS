# is_string

Comprueba si un valor es una cadena de texto.

## Sintaxis

  
```gml  
is_string(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El valor a comprobar.|  

## Descripción

Esta función comprueba si un valor dado es de tipo cadena de texto. En algunas ocaciones puede llegar a ser necesario saber si una variable almacena una cadena de texto o no, y en estos casos esta función es de utilidad. Devuelve `true` o `false` dependiendo si el tipo de dato es una cadena de texto o no.

## Devuelve

Booleano

## Ejemplo

  
```gml  
datos[0] = "Una cadena";  
datos[1] = "Otra cadena";  
datos[2] = 32;  
datos[3] = "Otra más";  
datos[4] = false;  
datos[5] = spr_Enemigo;  
  
for(i = 0; i < 6; i++) {  
    if(is_string(datos[i]))  
        show_message("¡Es una cadena!");  
    else show_message("No es una cadena :(");  
}  
```  
Se crea un array con 6 índices diferentes, y se usa un ciclo para comprobar si cada índice almacena una cadena o no. Los mensajes que se mostrarían serían, en este orden, `"¡Es una cadena!"`, `"¡Es una cadena!"`, `"No es una cadena :("`, `"¡Es una cadena!"`, `"No es una cadena :("` y `"No es una cadena :("`.