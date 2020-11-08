# game_restart

Reinicia el juego.

## Sintaxis

  
```gml  
game_restart();  
```  

## Argumentos

Ninguno

## Descripción

Esta función permite reiniciar el juego. Al ejecutarse, también se ejecutará el evento **Game End**. Igualmente, al reiniciarse el juego será, en escencia, igual a como si se estuviera ejecutando por primera vez, lo que significa que también se ejecutará el evento **Game Start**. Sin embargo, las variables globales no será re-inicializadas automáticamente. Por ejemplo, la variable `score` no iniciará en 0 después de reiniciar el juego si ésta se ha modificado anteriormente.

## Devuelve

Nada.

## Ejemplo

  
```gml  
if keyboard_check_pressed(ord("R"))  
    game_restart();  
```  
Si se presiona la tecla **R**, se reiniciará el juego.