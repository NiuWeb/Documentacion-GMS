# cursor_sprite

Asigna un _sprite_ como cursor.

## Sintaxis

  
```gml  
cursor_sprite;  
```  

## Argumentos

Ninguno

## Descripción

Con esta variable es posible establecer un sprite del juego como el cursor del mismo. El valor por defecto es -1, que indica que no se dibujará ningún sprite como cursor. Cabe mencionar que no es posible tomar control de la animación del sprite con esta variable; si el sprite establecido tiene subimágenes, la animación se repetirá a la misma velocidad de la sala.  
  
Cabe mencionar que esta variable **no** reemplaza el cursor de la ventana del juego, y éste continuará dibujándose normalmente.

## Devuelve

Número real.

## Ejemplo

  
```gml  
cursor_sprite = spr_gameCursor;  
```  
Se establece como cursor el sprite `spr_gameCursor`.