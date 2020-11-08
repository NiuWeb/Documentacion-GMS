# surface_reset_target

Establece el objetivo de dibujado de nuevo a la pantalla, que es la predeterminada.

## Sintaxis

  
```gml  
surface_reset_target();  
```  

## Argumentos

Ninguno

## Descripción

Con esta función restablece todo el dibujado posterior a la fijación de una surface, de nuevo a la pantalla. Por favor tener en cuenta que para dibujar en una surface primero debe ser llamada la función `surface_set_target()` y luego al terminar de usarla debe de restablecer el objetivo para cada surface puesta como objetivo de dibujado, de lo contrario en pantalla no sera dibujado nada (incluso otras instancias se verán afectadas) por que se dibujará en la surface. También debe tener en cuenta que no se verá la surface, si no esta siendo dibujada en pantalla en el evento draw de una instancia.  
  
_**Nota:** si anteriormente no se a cambiado el objetivo de dibujado con la función `surface_set_target`, esta función se ejecutará de forma silenciosa (sin ningún mensaje de error) y se terminara de forma normal el código que se este ejecutando en el evento._

## Devuelve

Nada

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
El código anterior comprueba que view se esta dibujando actualmente, si es view[0] establece el objetivo de dibujado a una surface y dibuja sobre ella todas las instancias del objeto "obj_Effect" antes de restablecer el objetivo de dibujado. Si la vista no es view[0], dibuja la surface en la pantalla.