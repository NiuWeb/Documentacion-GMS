# Anexo: Introducción a las partículas

## ¿Qué son las partículas?

Las partículas son recursos gráficos que tienen ciertas propiedades definidas dentro de un sistema de partículas. Esas propiedades no se pueden manipular directamente en partículas individuales, sino que se manejan a través del código usado para definir el tipo de partícula y el sistema al que pertenece. Son muy útiles para crear efectos hermosos y llamativos (o sutiles y discretos si se desea) como explosiones, huellas, lluvia, nieve, campos de estrellas y escombros sin una carga excesiva a la CPU.

La preparación básica de un sistema de partículas se hace en tres pasos, siendo el tercer paso opcional:

*   **Crear un sistema de partículas:** El sistema de partículas es como un contenedor para nuestros diferentes tipos de partículas. Se usa código para definir una serie de aspectos visuales y de comportamiento para las partículas, y entonces se colocan en el "contenedor" de forma que podemos tomarlas y usarlas en donde las necesitemos después.
  
*   **Crear tipos de partículas:** Se pueden definir diferentes tipos, cada uno con su propio rango de colores, opacidad, tamaños y movimientos, pero es importante resaltar que no se puede tener control sobre partículas individuales. Se define una serie de parámetros y las partículas serán creadas con valores al azar dentro del rango de parámetros.
  
*   **Crear emisores:** Los emisores se pueden usar para crear un estallido de partículas o un flujo constante de partículas dentro de un área claramente definida. Son opcionales porque las partículas también se pueden crear con las funciones `part_particles_create` y `part_particles_create_colour`, pero no son adecuadas para todas las situaciones.

## Limitaciones

Aunque las partículas son una excelente herramienta para crear efectos visuales, tienen ciertas restricciones y se deben seguir ciertas prácticas para evitar ralentizar el juego y llegar al punto en que deje de funcionar:

*   Los sistemas de partículas, los emisores y las partículas ocupan memoria, y es fácil causar una fuga de memoria que ralentizará y finalmente cerrará el juego. Una manera de enfrentar esto es tener un sistema global con todo definido al principio del juego y removerlo al final, pero si se desea un sistema "dinámico" entonces cada partícula y emisor deben ser destruidos en el momento en que ya no son necesarios.
  
*   Las partículas son rápidas y ligeras para la CPU, pero aun así requieren algo de procesamiento y por lo tanto no se deberían tener 40000 de ellas generándose a cada momento. Intente limitarlas a las mínimas necesarias para crear un efecto.
  
*   Si define una partícula con sprite personalizado, el sprite debe ser lo más pequeño posible para lograr el efecto deseado.
  
*   Las partículas no interactúan con objetos ni con otras partículas. Si se requiere algún tipo de interacción se deben usar instancias. En GM8 hay funciones para simular la interacción, pero fueron eliminadas porque incrementan demasiado la carga del procesador.
  
*   No existe un límite técnico para el número de sistemas, emisores y partículas que se pueden crear en un juego, pero se debe usar lo mínimo para usar la menor cantidad de memoria posible.
  
*   En dispositivos móviles, dibujar partículas puede ser lento si cubren un área grande de la pantalla, esta es una de las principales causas de ralentización.
  
*   En HTML5, para usar “mezcla aditiva” (additive blending) se debe activar WebGL, sin embargo, no se puede usar “mezcla de color” (colour blending).

## Herramientas

Para diseñar efectos con partículas en tiempo real, y para estudiar esta sección del manual, es conveniente utilizar un programa “diseñador de partículas”. A continuación se muestra una lista de programas, algunos son gratis y otros no. El primero es muy bueno porque tiene una versión que se puede ejecutar en el navegador:

*   [PixelCandy (ZiNGOT)](https://marketplace.yoyogames.com/assets/3976/pixelcandy)
*   [Particle Designer 2.5 (Alert Games)](http://alertgames.net/old/?page=s/pd2)
*   [Simple Particle Designer (Posva)](http://www.comunidadgm.org/index.php?page=JuegosOnline&accion=ver&id=87)
*   [Geon FX (Steam Panic)](http://www.steampanic.com/geonfx/)
*   [TMC Particle Lab (The Mojo Collective)](http://themojocollective.com/Main/TMC%20Apps%20pages/TMC_Particle_Lab.htm)