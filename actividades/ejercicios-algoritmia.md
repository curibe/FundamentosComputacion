---
description: >-
  Se proponen algunos problemas para resolver en donde debe usar lo visto en la
  unidad de algoritmia. Los ejercicios van a tener diferentes dificultades
---

# Ejercicios Algoritmia

1. Dada la base y altura de un triangulo, calcular el area y perímetro
2. Dados los valores de a,b y c de la desigualdad $$|ax-c|<c$$ , determinar el intervalo en el que se encuentra x.
3. Dados dos puntos $$P1:(x_1,y_1)$$ y $$P2:(x_2,y_2)$$ , determinar la ecuación de la recta tangente.
4. Dado un valor N suministrado por el usuario, determinar la suma de los N primeros números naturales. _Sugerencia: use la suma de Gauss._
5. Determinar el area y el volumen de las siguientes figuras:  a\)Cilindro b\) Piramide de base rectangular c\) Esfera d\) Piramide de base triangular e\) Casquete esferico  El algoritmo debe permitir al usuario escoger entre las opciones anteriores, y dependiendo de la opcion que escojan, se le debe pedir que ingrese los parámetros necesarios para calcular ambas cantidades.
6. Escribir un algoritmo en el que dada una cantidad N de numeros, determine el valor promedio del conjunto de números.
7. Dado dos valores ingresados por el usuario, determinar cual es el mayor y el menor
8. Dado un conjunto de N numeros ingresados por el usuario, determinar cual es el mayor y el menor de todos
9. Dado un numero $$n$$ingresado por el usuario, determinar si es primo o no. 
10. Dado un numero N, determinar los N primeros números primos
11. Dado dos valores M y N , con M&gt;N, determinar $$M$$es multiplo de $$N$$
12. Se tiene que en un parqueadero de vehículos \(motos y carros\)la hora de parqueo para un carro es de $4000 y para una moto de $2000, las dos primeras horas de parqueo. Despues de las dos primeras horas, se cobra la hora a $2000 y $ 1500, sin embargo, si la estadía del vehículo no es la hora completa, se le cobra de a fracci\[on de 15 minutos. Escribir un algoritmo en el que dado el tipo de vehiculo, la hora de entrada y la hora de salida, de el valor que tiene que pagar por el parqueo. Recuerde que debe tener en cuenta las fracciones de tiempo \(de a 15min\) que dure el vehiculo en el parqueadero.
13. Escriba un algoritmo en el que dado 5 números enteros, determine cual de los cuatro últimos números es mas cercano al primero. \(Por ejemplo, si el usuario introduce los numeros 2,6,4,1 y 10, el  programa debe responder que el numero mas cercano a 2 es 1\)
14. Escribir un algoritmo en el que dado dos puntos $$P1:(x_1,y_1)$$ y $$P2:(x_2,y_2)$$del plano cartesiano, determinar la distancia de los dos puntos
15. Dado un conjunto de 5 puntos $$(x_i,y_i)\;_{i=1,..,5}$$ , determine cual de los ultimos cuatro puntos es mas cercano al primero.
16. Escriba un algoritmo en el que dado los números n y m, calcule el resultado de la siguiente expresion:

    $$
    \sum_{i=n}^m i
    $$

    n y m deben ser numeros enteros que deben ser ingresados por teclado y m debe ser mayor que n. El algoritmo debe validar las entradas \(verificar si m&gt;n\)

17. Dado un numero n, calcular el factorial de dicho numero: $$n!=1\cdot2\cdot3\cdots(n-1)\cdot n$$ . Debe tener en cuenta que n debe ser un entero positivo y que 0!=1. El algoritmo debe validar de que el valor de n ingresado sea positivo.
18. El numero de combinaciones que se puede formar tomando m elementos de un conjunto de n elementos es:

    $$
    C_m^n=\binom{n}{m}=\dfrac{n!}{(n-m)!m!}
    $$

    Escriba un algoritmo donde se pida el valor de n y m y calcule  $$C_m^n$$ . Tenga en cuenta que n&gt;m.

19. Escribir un algoritmo en el que dado un numero $$n$$, se muestren en pantalla los primeros N numeros pares. Verifique numéricamente que: $$1+2+4+\cdots+2^n)=2^{n+1}-1$$
20. Escribir un algorimot en el que dado un numero N, se muestren en pantalla los primerons N numeros impares. Verifique numericamente que: $$1+3+5+\cdots+(2n-1)=n^2$$ 
21. Dado un número n, calcular la siguiente suma y verificar que se cumple que:

    $$
    1^2 + 2^2 + 3^2+4^2 + \cdots +n^2=\dfrac{n(n+1)(2n+1)}{6}
    $$

22. Dado un numero $$N$$, determinar los $$N$$primeros numeros de la sucesión de fibonacci
23. Dado un numero en formato binario, convertir a decimal
24. Dado un número en decimal, convertir en binario
25. Dado dos numeros complejos $$z_1,z_2$$, calcule la suma, la resta ,la multiplicacion y la division entre ambos.
26. Elaborar un algoritmo en el que dado un valor de tiempo en segundos, diga cuantas horas minutos y segundos corresponde.
27. Un computador solo sabe sumar/restar, multiplicar y dividir. El calculo de muchas funciones complicadas en la fisica se hace recurriendo al uso de las llamadas series de potencias. Por ejemplo,una funcion tan comun como $$\sin(x)$$ puede calcularse usando la suma infinita:

    $$
    \sin(x)=x-\frac{x^3}{3!}+\frac{x^5}{5!} - \frac{x^7}{7!} + \cdots
    $$

    La suma produce un resultado finito si $$x$$ \(en radianes\) es relativamente pequeño \($$x < 1$$\). Obviamente un computador nunca podría realizar una suma infinita y lo que se hace regularmente es calcular la suma hasta el termino n-esimo y suponer que lo que queda de la misma es muy pequeño! Elaborar un algoritmo en el que dados $$x$$ y el número de términos a utilizar de la serie calcule el seno de $$x$$

28. Elabore un algoritmo en el que dado un ángulo en decimal \(por ejemplo: $$65.786\degree$$ \) indique las tres partes del angulo en sexagesimal \(grados,minutos y segundos\).
29. Elaborar un algoritmo en el que dado un angulo dado en sexagesimal, se obtenga el valor decimal de este.
30. Cuando en un circuito electrico se tienen resistencias conectadas en serie o en paralelo, estas pueden ser reemplazadas por una resistencia equivalente que cumple la misma función que el conjunto de resistencias. Cuando las resistencias estan conectadas en serie, la resistencia equivalente se puede obtener de la siguiente forma:  
  
    $$R_{eq}= R_1 + R_2 + R_3 + \cdots + R_N$$,  donde $$N$$es el número de resistencias  
  
    y si estan conectadas en paralelo seria de la siguiente forma:

    $$
    \frac{1}{R_{eq}}=\frac{1}{R_{2}}+\frac{1}{R_{2}}+\frac{1}{R_{3}}+\cdots+\frac{1}{R_{N}}
    $$

    Dado un numero $$N$$de resistencias, calcular la resistencia equivalente de este conjunto cuando estan conectadas en serie y en paralelo. Los valores de la resistencia deben ser ingresados por teclado.

31. Escribir un algoritmo que calcule el valor aproximado de $$\pi$$usando la siguiente serie:

    $$
    \frac{\pi^2}{6}=\frac{1}{1^2}+\frac{1}{2^2}+\frac{1}{3^2}+\frac{1}{4^2}+\cdots
    $$

32. Escribir un algoritmo que calcule el valor aproximado de $$\pi$$usando la siguiente serie:

    $$
    \frac{2}{\pi}=\frac{\sqrt{2}}{2}\cdot \frac{\sqrt{2+\sqrt{2}}}{2}\cdot \frac{\sqrt{2+\sqrt{2+\sqrt{2}}}}{2}\cdots
    $$

    El algoritmo debe recibir el número $$N$$de factores que se deben usar. Si $$N$$es igual a 3 debe usar los terminos que se usan en la formula anterior.

33. Escriba un algoritmo en el que dado un numero $$x\; (x<1)$$y un numero natural $$N$$, calcule el valor del seno inverso usando los primeros $$N$$terminos de la serie:

    $$
    \arcsin z= z + \left(\dfrac{1}{2}\right)\dfrac{z^3}{3} + \left(\dfrac{1\cdot3}{2\cdot4}\right)\dfrac{z^5}{5} + \left(\dfrac{1\cdot3\cdot5}{2\cdot4\cdot6}\right)\dfrac{z^7}{7}+\cdots
    $$

34. Escribir un algoritmo que calcule el valor de la siguiente formula

    $$
    \dfrac{4}{1+\dfrac{1^2}{3+\dfrac{2^2}{ 5+\dfrac{3^2}{ 7+\dfrac{4^2}{ 9+ \cdots} } }}}
    $$

    El algoritmo debe recibir como entrada el numero $$N$$de divisiones para calcular. Si $$N=2$$debe calcular hasta $$4/(1+1/3)$$. ¿Cual es el valor calculado?

35. Dado un valor de $$x$$, calcular $$\exp (x)$$por medio de la siguiente expresión:

    $$
    \exp(x)=e^x=1+x+\frac{x^2}{2!}+\frac{x^3}{3!} + \cdots
    $$

36. Ecribir un algoritmo en el que dada la veloci de lanzamnto de un proyectil y el angulo que forma con la horizontal, calcule y muestre el alcance, la altura maxima y el tiempo de vuelo.
37. Un cuerpo de 1 kg de masa se suelta desde una altura de 1000 m en un lugar donde la aceleración de la gravedad es de $$9.8\; m/s^2$$. Utilice las formulas generales para la caida libre:  $$y=y_0+v_0-\dfrac{1}{2}gt^2; \qquad v=v_0-gt$$  y las formulas para la energia cinética \($$E_c$$\)y la energia potencial $$(E_p)$$:  $$E_c=\dfrac{1}{2}mv^2; \qquad E_p=mgy$$  para escribir un algoritmo que muestre en pantalla una tabla con las siguientes columnas: tiempo,distancia, velocidad, energia cinetica, energia potencial y la suma de estas dos energias \(Energia mecanica total\) hasta cuando la particula llegue al piso. 
38. Verifique numéricamente la siguiente expresion matematica:

    $$
    e =\lim_{n \to \infty} \left(1+\dfrac{1}{n}\right)^n
    $$

    Escriba un agoritmo que tome valores de $$n=1,10,20,50,100,500,1000$$y verifique que se acerca al valor de $$e$$. Mediante la libreria _math_ de python, compare su resultado para cada valor de $$n$$con el valor de $$e$$de la libreria _math_ y muestre el porcentaje de error. ¿cuantos terminos cree que debe agregar para tener un valor con una precision de 4 cifras decimales?

39. Compruebe de forma numerica la paradoja de Zenon  $$\hspace{3.5cm} \dfrac{1}{2}+\dfrac{1}{2^2}+\dfrac{1}{2^3}+\dfrac{1}{2^4}+\cdots=1$$ 
40. 






