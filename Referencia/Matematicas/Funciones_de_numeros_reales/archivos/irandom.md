# irandom

Devuelve un número entero aleatorio entre cero y el número dado.

## Sintaxis

  
```gml  
irandom(n);  
```  

## Argumentos

Argumento|Descripción|  
---|---|  
n|El número límite para generar.|  

## Descripción

Esta función permite obtener un número entero aleatorio entre cero y `n`. El número argumentado **puede** ser generado. Esta función tiene un límite máximo de **$7fffffffffffffffLL**, por lo que es necesario tener cuidado al trabajarla con números grandes.  
  
**NOTA:** Esta función generará los mismos resultados (en el mismo orden) cada vez que se ejecuta el juego. Esto gracias a que Game Maker Studio genera la misma semilla aleatoria inicial. Para evitar esto, usar `randomize()` al inicio del juego para generar una nueva semilla aleatoria.

## Devuelve

Número entero.

## Ejemplo

  
```gml  
a = irandom(10); //Genera un número aleatorio entre 0 y 10. El número 10 puede ser generado.  
if(a == 5) {  
    show_message("¡Has ganado un premio!");  
}  
```  
Se hace uso de `irandom()` para crear una probabilidad del 10% de que se muestre un mensaje emergente que diga `"¡Has ganado un premio!"`.