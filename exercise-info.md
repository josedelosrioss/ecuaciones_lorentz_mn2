Las ecuaciones de Lorenz
El sistema de Lorenz es un conjunto de tres ecuaciones diferenciales ordinarias, desarrollado inicialmente por el meteorólogo Edward Lorenz mientras estudiaba la convección atmosférica. Es un ejemplo clásico de un sistema que puede exhibir un comportamiento caótico, lo que significa que su resultado puede ser altamente sensible a pequeños cambios en sus condiciones iniciales.

Para ciertos valores de sus parámetros, las soluciones del sistema forman un patrón complejo y cíclico conocido como el atractor de Lorenz. Se dice que la forma de este atractor, al ser representada, se parece a una mariposa. La extrema sensibilidad del sistema a las condiciones iniciales dio origen al popular concepto del efecto mariposa: la idea de que un pequeño evento, como el aleteo de una mariposa, puede alterar los patrones climáticos a gran escala. Si bien el sistema es determinista (su comportamiento futuro está completamente determinado por sus condiciones iniciales), su naturaleza caótica hace que la predicción a largo plazo sea prácticamente imposible.


En 1963, Edward Lorenz desarrolló el sistema como un modelo matemático simplificado para la convección atmosférica. Intentaba modelar el movimiento del aire cuando se calienta desde abajo y se enfría desde arriba. El modelo describe cómo cambian con el tiempo tres propiedades clave de este sistema:

x
 es proporcional a la intensidad de la convección (la velocidad del flujo de fluido).
y
 es proporcional a la diferencia de temperatura entre las corrientes de aire ascendentes y descendentes.
z
 es proporcional a la desviación del perfil de temperatura vertical respecto a un perfil lineal.

El comportamiento de estas tres variables se rige por las siguientes ecuaciones, cuyos valores cambian con el tiempo, definido como t
:

dx/dtdy/dtdz/dt===σ(y−x)x(ρ−z)−yxy−βz

 Las constantes  ρ,σ
 y β
 son parámetros que representan propiedades físicas del sistema: σ
 es el número de Prandtl, ρ
 es el número de Rayleigh y β
 se relaciona con las dimensiones físicas de la capa de fluido.

El comportamiento del sistema depende de la elección de los parámetros. Para ciertos rangos de parámetros, el sistema es predecible: las trayectorias se estabilizan en puntos fijos u órbitas periódicas simples, lo que facilita la descripción del comportamiento a largo plazo. Por ejemplo, cuando ρ<1
, todas las soluciones convergen al origen, y para ciertos valores moderados de ρ,σ
 y β
, las soluciones convergen a estados estacionarios simétricos.

En cambio, para otros rangos de parámetros, el sistema se vuelve caótico. Con los parámetros conocidos σ=10,ρ=28,β=8/3
 las soluciones nunca se estabilizan, sino que trazan el atractor de Lorenz con forma de mariposa. En este régimen, pequeñas diferencias en las condiciones iniciales crecen exponencialmente.

Desde un punto de vista técnico, el sistema de Lorenz es no lineal, aperiódico, tridimensional y determinista. Aunque originalmente se aplicaron al clima, se ha descubierto que las ecuaciones modelan el comportamiento en una amplia variedad de sistemas, incluidos láseres, dinamos, circuitos eléctricos, e incluso algunas reacciones químicas.

Problema
Utilice el método de Runge-Kutta clásico con longitud de paso h=0.01
 para resolver las ecuaciones de Lorenz en el intervalo [0,100]
, con condiciones iniciales (x0,y0,z0)=(3,15,1)
, para los valores de los parámetros σ=10,ρ=28,β=8/3
. Represente las soluciones aproximadas de las ecuaciones de Lorenz.
Repita el mismo procedimiento con distintas condiciones iniciales. Comente el resultado.
Repita el proceso para los valores de los parámetros  σ=10,ρ=14,β=8/3
 y  σ=10,ρ=99.6,β=8/3
. Comente el resultado.
Instrucciones para la entrega
Se valorará la creatividad en la práctica añadiendo aportes personales. Por ejemplo, sería interesante poder seleccionar la zona del espacio donde se dibuja, cambiar el enfoque de cámara, crear animaciones ilustrando el avance de las iteraciones, ...
La práctica puede realizarse en grupo. El número máximo de integrantes del grupo es de tres estudiantes.
La entrega se realiza mediante la subida a la correspondiente tarea de Prado de un único notebook de Jupyter que contenga tanto el código en Python como los resultados e imágenes obtenidos.
El código debe estar correctamente documentado.
