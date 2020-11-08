# game_end

Cierra el juego.

## Sintaxis

  
```gml  
game_end();  
```  

## Argumentos

Ninguno

## Descripción

Esta función permite finalizar el juego (y ejecutar el evento **Game End**). Esta acción no se lleva a cabo inmediatamente al ejecutarse, sino al final del _step_ actual. Por ello, cualquier código que se tenga en el mismo _step_ que la función ha sido llamada, continuará ejecutándose. Esta función tiene ciertas condiciones:  

*   En los módulos **Windows 8** e **iOS** se reportará un error, como está establecido en las condiciones de sus respectivas tiendas.
*   No funciona en el módulo HTML5
*   Trabaja correctamente en las plataformas **Windows** (incluyendo _Steam Workshop_), **Windows Phone**, **Android**, **Linux** y **Mac**.

## Devuelve

Nada

## Ejemplo

  
```gml  
if(keyboard_check_pressed(vk_escape))  
    game_end();  
```  
Si se presiona la tecla escape, se cerrará el juego.