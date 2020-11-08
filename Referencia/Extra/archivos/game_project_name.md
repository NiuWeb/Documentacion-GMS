# game_project_name

Devuelve el nombre del juego establecido en _**Global Game Settings**_.

## Sintaxis

  
```gml  
game_project_name;  
```  

## Argumentos

Ninguno

## Descripción

Esta función permite obtener el nombre del juego establecido en _**Global Game Settings**_ para la plataforma en la que se está ejecutando actualmente. Probablemente esta variable devuelva lo mismo que `game_display_name`, excepto que de contener algún caracter especial, lo reemplazará por un guion bajo (`"_"`).

## Devuelve

Cadena de texto.