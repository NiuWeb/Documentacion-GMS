# surface_set_target

Establece el objetivo de dibujado a una surface especifica.

## Sintaxis

  
```gml  
surface_set_target(surface_id);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
surface_id|El ID de la surface a establecer como objetivo de dibujado.|  

## Descripción

Esta función establece todo el dibujado a una surface seleccionada en lugar de la pantalla, de esta manera puede decirle a GameMaker: Studio que dibuje cosas especificas sobre la surface. Tenga en consideración que de no llamar la función `surface_reset_target()` después de haber terminado, no se dibujará nada en la pantalla ya que todo el dibujado (incluido el de otras instancias) se realizará sobre la superficie. También considere que no se verá la surface si esta no es dibujada en un evento draw de una instancia. Puede comprobar el valor devuelto por esta función para comprobar si la surface se estableció correctamente o no; un valor de 0 es igual a un fallo y cualquier otro numero positivo es correcto.  
  
Un dato importante a tener en cuenta es que las surface se apilan, por lo que no puede saltar de una surface fijada como objetivo a la pantalla por defecto, sino que debe abrir y cerrar todos los cambios de objetivo de dibujado. Ejemplo, esto no funcionará correctamente:  
  
```gml  
surface_set_target(surf1);  
draw_text(32, 32, "surface1");  
surface_set_target(surf2);  
draw_text(32, 64, "surface2");  
surface_reset_target();  
  
```  
  
Para que funcione correctamente debe de restablecer el objetivo de dibujado para cada surface que establece, al igual que debe de usar los corchetes **{}** para los bloques de código. Así que lo anterior debe de escribirse como lo siguiente:  
  
```gml  
surface_set_target(surf1);  
draw_text(32, 32, "surface1");  
surface_reset_target();  
surface_set_target(surf2);  
draw_text(32, 64, "surface2");  
surface_reset_target();  
  
```  
  
O así:  
  
```gml  
surface_set_target(surf1);  
draw_text(32, 32, "surface1");  
surface_set_target(surf2);  
draw_text(32, 64, "surface2");  
surface_reset_target();  
surface_reset_target();  
  
```  
  
_**Nota:** Cuando se trabaja con surface existe la posibilidad que se destruyan en cualquier momento. Debe **siempre** comprobar si existen con `surface_exists()` antes de hacer algo con ellas._

## Devuelve

Boleano

## Ejemplo

  
```gml  
if view_current = 0{  
     surface_set_target(surf);  
     with (obj_Effect){  
          draw_self();  
     }  
     surface_reset_target();  
}  
else{  
     draw_surface(surf, 0, 0);  
}  
```  
El código anterior comprueba la vista actual que esta siendo dibujada, si esta es la view[0] establece el objetivo de dibujado a una surface y dibuja todas las instancias del objeto "obj_Effect" antes de restablecer el objetivo de dibujado. Si la vista no es la view[0] la surface es dibujada en pantalla.