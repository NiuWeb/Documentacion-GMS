# ini_close

Cierra el archivo ini abierto actualmente.

## Sintaxis

  
```gml  
ini_close();  
```  

## Argumentos

Ninguno

## Descripción

En caso de haber terminado de leer o escribir toda la información necesaria de un archivo ini previamente abierto, es necesario ejecutar esta función para cerrarlo. Mientras esta función no sea llamada, la información escrita en el archivo no será guardada en el mismo. De igual forma, si se intenta abrir un archivo ini sin antes haber cerrado otro, se ocacionará un error.  
  
Esta función también devuelve una cadena de texto con el contenido del archivo ini (incluyendo la información escrita antes de cerrar el archivo). Esta cadena puede, por ejemplo, guardarse en un servidor, o ser utilizada con `ini_open_from_string()` para poder manejar su información.

## Devuelve

Cadena de texto.

## Ejemplo

  
```gml  
ini_open("datos.ini");  
monedas = ini_read_real("datos", "monedas", 0);  
nivel = ini_read_real("datos", "nivel", 1);  
nombre = ini_read_string("datos", "nombre", "Player");  
ini_close();  
```  
Se abre el archivo datos.ini para lectura y escritura. Posteriormente se leen algunos datos del archivo y por último éste se cierra.