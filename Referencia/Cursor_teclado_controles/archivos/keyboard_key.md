# keyboard_key

Almacena la tecla que esta actualmente en uso.

## Sintaxis

  
```gml  
keyboard_key;  
```  

## Argumentos

Ninguno

## Descripción

Con esta variable puede obtener el código de la tecla que esta siendo actualmente presionada y devolverá 0 si no hay ninguna tecla presionada en el momento en que se comprueba.

## Devuelve

Entero

## Ejemplo

  
```gml  
switch (keyboard_key){  
     case vk_numpad1: gun = weapon[0,0]; break;  
     case vk_numpad2: gun = weapon[1,0]; break;  
     case vk_numpad3: gun = weapon[2,0]; break;  
}  
```  
El código anterior usa el valor de la variable `keyboard_key` para establecer una variable con un valor de un arreglo.