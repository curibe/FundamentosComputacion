---
description: Enero 27 - 2020
---

# PROYECTO FINAL - V2

### INDICACIONES

* El programa debe ser de su completa autoria, por lo que si su programa es una copia de alguna versión de internet \(la mas mínima copia\) o si lo manda a hacer, se le anula y le queda en cero. Pueden asesorarse de alguien pero deben ser ustedes quienes escriban el programa. Recuerden que cada persona tiene su propio estilo de programación, así que es muy fácil detectar fraude.
* Debe responder por escrito \(bien justificadas\) en el notebook cada una de las preguntas que se les hace ya que hace parte de la calificación. Recuerde que cada numeral lo debe resolver en una celda separada. No acepto todo el trabajo en una celda. 

**Fecha de de entrega:** Enero 30 de 2020 a las 18:00.



La integral tiene aplicaciones en muchas áreas como la estadística, la economía, las ciencias e ingeniería, puesto que nos permite calcular cantidades de interés como la fuerza que hace el agua sobre una represa, promedios de variables aleatorias continuas, masas, probabilidades entre muchas otras cantidades.

La integral nos permite calcula una cantidad, dividiéndola en partes muy pequeñas y sumando después la contribución de cada trozo. Por ejemplo, imagine que quiere calcular el volumen de un cuerpo deforme a partir de la densidad; una forma "practica" de hacerlo es coger el cuerpo y cortarlo en rebanadas y determinar el volumen de cada rebanada. Al final el volumen total del cuerpo va a ser la suma de cada volumen individual

![](https://upload.wikimedia.org/wikipedia/commons/3/31/Shell_integral_undergraph_-_around_y-axis.png)

Cuando es una función de una sola variable $$-f(x)-$$ , la interpretación geométrica de una integral _definida_ es el área bajo la curva $$f(x)\text{ vs }  x$$ . En este caso, se podría calcular el área bajo la curva \(note que la integral permite calcular el área de superficies irregulares\) dividiendo la zona en pequeños rectángulos, y calcular el área de cada rectángulo para poder tener el área total. Entre mas rectángulos se tenga, mas preciso va a ser el valor del área.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Riemann_Integration_and_Darboux_Upper_Sums.gif/640px-Riemann_Integration_and_Darboux_Upper_Sums.gif)

Hay muchas cantidades físicas que se relacionan con otras a través de una integral y muchas veces estas integrales no se pueden resolver de forma analítica. Por esta razón se recurre a métodos numéricos que permitan obtener el valor de ellas. Este método se conoce como el _método de los rectángulos._ Este método se puede emplear de distintas formas ya que la construcción de los rectángulos se puede hacer de 3 formas: _rectángulos internos, rectángulos externos, y rectángulos intermedios._

![](../.gitbook/assets/image%20%2838%29.png)

Para el caso en el que se usan los rectángulos intermedios, la integral queda dada como:

![](../.gitbook/assets/image%20%2855%29.png)

$$
\begin{eqnarray*}
\int_a^b f(x)dx &=& \sum_{k=1}^N \left( \Delta x f(x_k^*) \right) = \Delta x \sum_{k=1}^N  f(x_k^*)\\
                &=& \frac{b-a}{N}\left[f(x_1^*
)+f(x_2^*)+f(x_3^*)+\cdots + f(x_N^*) \right]
\end{eqnarray*}
$$

Un método un poco mas preciso que el anterior y también utilizado, es la conocida _Regla del Trapecio_, el cual no usa rectángulos sino trapecios para aproximar el área debajo de la curva

![](https://upload.wikimedia.org/wikipedia/commons/7/7e/Trapezium2.gif)

Para resolver una integral numérica por medio de la regla de los trapecios, se usa la siguiente definición del método:

para un dominio \(valores de $$x$$ \) discretizado en $$N$$ trapecios igualmente espaciados, o $$N+1$$ puntos $$a = x1 < x2 < ... < x_{N+1} = b$$ donde la separación entre cada valor de $$x$$ $$h=(b-a)/N$$ \(puede verlo como el ancho de caga trapecio en la figura de arriba\), la integral puede ser aproximada como:

$$
\begin{eqnarray*}
\int_a^b f(x)dx &=& \frac{h}{2}\sum_{k=1}^N \left( f(x_{k+1})+f(k) \right)\\
                &=& \frac{b-a}{2N}(f(x_1)+2f(x_2)+2f(x_3)+\cdots + 2f(x_N) + f(x_{N+1}))
\end{eqnarray*}
$$

NOTA: Compare la anterior expresión con la fórmula del área de un trapecio \(Ver imagen debajo\)



![](../.gitbook/assets/image%20%2854%29.png)

### PARTE 1-MÉTODO DEL RECTÁNGULO

**a\)** Hacer una rutina en python, en la cual implemente el método de los rectángulos expuesto anteriormente. Esta rutina debe recibir una función genérica, los valores de $$a$$ y $$b$$ así como el valor de $$\Delta x$$. En caso de que $$\Delta x$$ no se suministre, $$\Delta x$$ debe tomar un valor por defecto \( ¿cual cree que podría ser un valor por defecto? \). Consulte como se calcularía la suma de las áreas de los rectángulos cuando estos están por debajo y por encima.

**b\)** Para verificar si su rutina funciona correctamente, pruébela resolviendo la integral definida $$\int_0^5 \sqrt{x}$$.  Puede verificar el resultado [aqui!!](https://www.wolframalpha.com/input/?i=integral%5Bsqrt%28x%29%2C%7Bx%2C0%2C5%7D%5D). ¿ Con cuantos rectángulos obtiene un valor que coincida en 3 cifras decimales al valor real?

### PARTE 2-MÉTODO DEL TRAPECIO

**a\)** Hacer una rutina en python, en la cual implemente el método de los trapecios expuesto anteriormente. Esta rutina debe recibir una función genérica, los valores de $$a$$ y $$b$$ así como el valor de $$h$$. En caso de que $$h$$ no se suministre, $$h$$ debe tomar un valor por defecto \( ¿cual cree que podría ser un valor por defecto? \). Note que el método consiste en una suma de $$n$$ términos donde los términos están multiplicados por 2, excepto los valores extremos.

**b\)** Para verificar si su rutina funciona correctamente, pruébela resolviendo la integral definida $$\int_0^5 \sqrt{x}$$.  Puede verificar el resultado [aqui!!](https://www.wolframalpha.com/input/?i=integral%5Bsqrt%28x%29%2C%7Bx%2C0%2C5%7D%5D).¿ Con cuantos trapecios obtiene un valor que coincida en 3 cifras decimales al valor real?

**c\)** En física moderna, cuando se quiere calcular la energía electromagnética de una cavidad que contiene fotones en su interior, aparece una integral de la siguiente forma:

$$
\int_0^{\infty}\frac{x^3}{e^x-1}dx.
$$

Solucionando la anterior ecuación, por medio del uso de series, se llega a lo siguiente:

$$
\int_0^{\infty}\frac{x^3}{e^x-1}dx = 6\sum_{n=0}^{\infty}\frac{1}{(n+1)^4} = \frac{\pi^4}{15}
$$

Grafique la función $$x^3/(e^x-1)$$ en el intervalo $$x:[0,15]$$. Usted debe obtener un gráfico como el siguiente:

![](../.gitbook/assets/image%20%2821%29.png)

**OBS:** Tenga presente que la función presenta una indeterminación en el punto $$x=0$$. Pruebe con un x muy pequeño cercano a cero pero no comience en cero ya que el programa le sacara error de división por cero.

**d\)** Haciendo uso de la rutina de integración hecha en el item **a\)** , calcule el valor de la integral y compare con el valor real. Para el caso en el que el limite superior es "infinito" \(∞\), ud puede asignarle un valor a b finito, pero lo suficientemente grande. ¿Que tan grande cree ud que debe ser el valor de b para este problema?

**e\) ¿**Con cuantos trapecios obtiene un valor que coincida en 3 cifras decimales con el valor real?. Con este numero encontrado, haga uso de la rutina del método de los rectángulos escrita en el numeral _a_ de la parte 1, para calcula nuevamente la integral. Compare los dos resultados y diga cuales de los dos es mas preciso. \(Note que se uso el mismo numero de elementos, por lo que se pueden comparar los resultados.\)

### PARTE 3 - INTEGRACIÓN MONTECARLO

El nombre integración Monte Cario proviene del uso de "números aleatorios" \(en realidad, _seudoaleatorios_\). La idea es aproximar el área de una región observando el número de parejas ordenadas aleatorias que caen dentro de la región y el número de las que caen afuera \(ver imagen\). El método es más útil cuando el integrando tiene muchas oscilaciones, pues en este caso la integral es difícil de aproximar con los métodos tradicionales como el de la parte a.

![](../.gitbook/assets/image%20%2817%29.png)

En algunas situaciones se pueden usar una caja \(figura de la izquierda\) delimitada por los valores extremos de la función o se puede definir un recuadro que encierre la función \(figura de la derecha\). En ambos casos es necesario definir la caja para poder generar los pares de coordenadas dentro de dicha caja.

La integración por el método de montecarlo queda definida como:

$$
\int_a^b f(x) dx = \text{Area del Rectangulo} \times\dfrac{\text{puntos dentro}}{\text{total de puntos}} = f_{max}(b-a)\dfrac{N_d}{N_T}
$$

**a\)** Escribir una rutina  en python, en la cual implemente el método de montecarlo mencionado anteriormente. Esta rutina debe recibir una función genérica $$f(x)$$, los valores de $$a$$ y $$b$$ así como el número total de puntos $$N$$que se van a generar aleatóriamente. Para generar los números aleatorios puede usar la función _uniform_  de la sublibrería numpy para números aleatorios: [https://docs.scipy.org/doc/numpy-1.14.0/reference/generated/numpy.random.uniform.html](https://docs.scipy.org/doc/numpy-1.14.0/reference/generated/numpy.random.uniform.html)

**b\)** Para verificar si su rutina funciona correctamente, pruébela resolviendo la integral definida $$\int_0^5 \sqrt{x}$$.  Puede verificar el resultado [aqui!!](https://www.wolframalpha.com/input/?i=integral%5Bsqrt%28x%29%2C%7Bx%2C0%2C5%7D%5D). Ensaye con distintos valores de $$N$$para determinar cual resultado se acerca mas al resultado obtenido en el numeral _b_ de la parte 1.

**c\)** Grafique la función $$x^3/(e^x-1)$$ en el intervalo $$x:[0,15]$$junto con los puntos generados aleatóriamente. Los puntos dentro de la curva deben ser de distinto color de los puntos por fuera. Pruebe con $$N=1000$$. Para esto, hágase las siguientes preguntas primero:  ¿ De que forma cree que se pueden determinar los puntos que están por debajo de la curva y los que están encima? ¿ cual condición cree que debe  cumplir un punto para que este por debajo de _f\(x\)_? Explique. El gráfico que debe obtener debe ser similar al siguiente

![](../.gitbook/assets/image%20%286%29.png)

Tenga presente que como los puntos son aleatorios, las gráficas no son exactamente las mismas, varia cada vez que ejecute todo el programa.

**d\)** Usando la función creada en el numeral a, pruebe con distintos valores de $$N$$. Pruebe con $$N=100,500,1000,5000,10000,20000,50000,70000,100000$$. Se debe mostrar cada uno de estos resultados como una tabla y que se compare con el valor real \(error absoluto\). Por ejemplo:

```text
==================================================
N          montecarlo          error       
==================================================
100        6.52499565        0.03105625    
500        6.25499583        0.23894357    
1000       6.20999586        0.28394354    
5000       6.54749564        0.05355623    
10000      6.43724571        0.05669369    
20000      6.47099569        0.02294372    
50000      6.42959571        0.06434369    
70000      6.49349567        0.00044373 
```

Tenga presente que estos resultados varían con cada ejecución ya que cada vez se generan números seudoaleatorios diferentes. En algunas situaciones cierto numero de puntos resultan ser mas precisos pero si se repite la ejecución, no. En la tabla anterior, en la ejecución hecha, $$N=70000$$da una cantidad que coincide con la real, pero si vuelve a ejecutar el código, probablemente ya solo coincida en 2 cifras.    ¿ Cuantos puntos cree que se necesita para obtener un resultado que coincida en 2 o 3 cifras decimales? ¿Con cuantos puntos se obtendría un resultado mas o menos estable?. Pruebe con valores de $$N$$mas grande pero increméntelos de forma paulatina \(no exageren en el valor de $$N$$\)

