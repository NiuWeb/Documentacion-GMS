# effect_create_below

Crea un efecto simple de partículas con profundidad 100000.

## Sintaxis

  
```gml  
effect_create_below(kind, x, y, size, colour);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
kind|Tipo de efecto (ver [lista de constantes](anexo_constantes_para_efectos_simples.html))|  
x|Posición X del efecto (si aplica)|  
y|Posición Y del efecto (si aplica)|  
size|Tamaño del efecto|  
colour|Color del efecto|  

## Descripción

Esta función crea un efecto simple con **profundidad positiva 100000**. Si el efecto es diferente a `ef_rain` o `ef_snow`, entonces se puede definir la posición y el tamaño del efecto. El tamaño puede ser 0, 1 o 2, donde 0 es pequeño, 1 es mediano y 2 es grande.  
  
El sistema de partículas para esta función tiene **índice 0**. El índice se puede usar para desactivar el dibujado automático y pausar la evolución del efecto con las funciones `part_system_automatic_draw` y `part_system_automatic_update`. El índice para `effect_create_above` es 1.

## Devuelve

Nada

## Ejemplo

  
```gml  
if( speed > 0 ){  
    effect_create_below(ef_smoke, x, y, 0, c_gray);  
}  
          
```  
El código anterior crea una nube de humo gris en cada Step, si la velocidad de la instancia es mayor a cero, generando una trayectoria de humo.