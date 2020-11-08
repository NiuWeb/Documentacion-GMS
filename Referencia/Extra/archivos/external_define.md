# external_define

Define una función externa.

## Sintaxis

  
```gml  
external_define(dll, name, calltype, restype, argnumb, argtype[0, ..., 10]) ;  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
dll|El nombre del archivo DLL del cual obtener la función. (Una cadena de texto).|  
name|El nombre de la función a obtener de la DLL. (Una cadena de texto).|  
calltype|El tipo de llamada a usar.|  
restype|El tipo de resultado que se espera.|  
argnumb|El número de argumentos (de 0 a 10).|  
argtype[0, ..., 10]|El tipo de dato que se usará en cada argumento.|  

## Descripción

Esta función permite definir una función externa desde un archivo _dll_ (para windows) o _dylib_ (para Mac). Este archivo puede encontrarse tanto en un archivo incluído como en una extensión. Se ingresa el nombre (incluyendo la ruta) del archivo, y posteriormente el nombre de la función a definir. Luego, es necesario establecer el tipo de llamada a utilizar, el cual es una de las siguientes constantes:  
  
Constante|Descripción|  
---|---|  
dll_cdecl|La llamada a C/C++ por defecto|  
dll_stdcall|La llamada a WinAPI estándar (sólo para _dll_'s windows)|  
  
  
Después, se ingresa el tipo de dato que se espera la función externa devuelva; puede ser `ty_real` si se espera un número real, o `ty_string` si se espera una cadena de texto. Lo siguiente es establecer el número de argumentos que se deben ingresar a la función externa, puede ser un número de 0 a 10. Por último, también se debe especificar el tipo de dato que se espera sea cada argumento que se ingresará a la función externa, utilizando las mismas constantes anteriores. Para funciones externas que requieran más de 4 argumentos, todos estos deben ser de tipo real.  
  
**NOTA:** Si la _dll_ o _dylib_ se encuentra en una extensión, las funciones externas deben definirse dentro de la extensión también.

## Devuelve

Nada.

## Ejemplo

  
```gml  
external_define("funciones_extra.dll", "repetir_cadena", dll_cdecl, ty_real, 2, ty_string, ty_real);  
```  
Se define una función externa llamada `"repetir_cadena"` que se encuentra dentro del archivo `"funciones_extra.dll"`. El tipo de llamada es `dll_cdecl` y la función tiene que devolver un número real. Posee dos argumentos, el primero es una cadena de texto y el segundo un número real.