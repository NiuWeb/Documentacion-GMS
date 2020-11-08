# math_set_epsilon

Establece el épsilon de la máquina

## Sintaxis

  
```gml  
math_set_epsilon(val);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
val|El nuevo valor del épsilon (de 0 a 0.999999999)|  

## Descripción

El épsilon es un valor utilizado para definir la precisión de las aproximaciones de cifras decimales, indica el mínimo margen de error en el que dos números pueden diferenciarse para considerarse iguales. Esta función es útil cuando se trabajan con cifras decimales pequeñas, para reducir los "errores de aproximación" que puedan ocacionar que las operaciones evalúen resultados incorrectos.  
  
Por ejemplo: Imaginemos que asignamos a la variable `image_index` de una instancia el valor de 5, el cual se espera ser un simple entero. Sin embargo, debido a la misma naturaleza de los números de punto flotante, el valor final de dicha variable podría terminar siendo algo como 5.0000002. Ahora bien, si tenemos la siguiente comprobación:  
  
```gml  
if(image_index == 5)  
{  
    //Hacer algo...  
}  
  
```  
La condición podría resultar ser falsa. Sin embargo, si definimos el épsilon a 0.000001, el valor de la variable será aproximado al número real más cercano en (+/-) 0.000001 del original, haciendo la comparación verdadera.  
  
**NOTA:** Si se define el épsilon como 0, se eliminará todo número decimal haciendo siempre comprobaciones con números enterios, mientras que definirlo como 1 ocasionará un error.

## Devuelve

Número real

## Ejemplo

  
```gml  
math_set_epsilon(0.001)  
```  
Se define la precisión decimal a 0.001.