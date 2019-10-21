# Ejercicios python

Se proponen algunos problemas para resolver y se debe escribir su respectivo programa en python. Hay algunas funcionalidades de python que pueden resolver el problema de forma rapida pero la idea resolver los problemas desde cero.

## Enunciados

**1\)**  Dado un conjunto de datos suministrados por el usuario, mostrar dicho conjunto en orden inverso.

**2\)**  Dado un conjunto de datos suministrados por el usuario de forma desordenada, organizar dicha secuencia de numeros de menor a mayor y mostrar en pantalla. Este es un algortimo de _sorting_; para este caso aplique el algoritmo [_quicksort_](http://sorting.at/) 

**3\)**  Elaborar un programa que calcule aproximadamente la longitud de una circunferencia de radio $$r$$   \(dado por el usuario\) a partir del perímetro de un polígono regular de $$n$$ lados \(dado también por el usuario\) inscrito en la circunferencia. ¿ Cuál es el valor de n para el cual el perímetro del polígono difiere del perímetro real de la circunferencia en un $$1\% $$ ?.  
**Sugerencia:** Tenga en cuenta que un polígono regular tiene lados iguales, ademas el angulo central $$\alpha$$ que subtiende cada lado es igual para todos. Por lo tanto, si un polígono tiene N lados, se tiene que:  
  
                                            $$\alpha = \dfrac{2\pi}{N}\; rad= \dfrac{360}{N} \; deg$$                         
  


![](../.gitbook/assets/image%20%2834%29.png)

**4\)**  Diseñe un programa que pida la entrada de un entero y que compruebe la conjetura de Goldbach: cada entero positivo mayor que dos puede escribirse como la suma de dos primos. **Sugerencia**: implemente el algortimo de numeros primos como una función.

**5\)**  Pitagoras sabia que los numeros 220 y 284 son _amigabls,_ es decir, que la summa de los factoresde uno es igual a la suma de los factores del otro. Escriba un programa que descomponga un entero en sus factores\(incluido el 1, pero no el numero mismo\), y que los sume para comprobar la _amistad_ de los numeros

**6\)**  Con el programa anterior encuentre el numero _amigo_ de 12285. nicolo paganini, en 1866 encontro que los numeros amigos mas pequeños qu siguen a 220 y 284 son 1184 y 1210; compruebelo.

**7\)**  En 1830, A. M. Lagrange publicó, pero sin poder demostrarlo, que si $$\pi(x)$$ es el número de primos menores o iguales al entero $$x$$, entonces $$\pi(x)$$  es aproximadamente igual a: $$x/(\log_ex-1.08366)$$.   
Compruebe esto con la rutina ue usted tiene para determinar si un entero es primo, e incorpore dicha rutina a un programa que lleve la cuenta de los numeros primos menores o iguales al numero dado

**8\)**  Los griegos buscaron números que al encontrarle los factores\(excepto el numero mismo\) y sumarlos, dieran el numero original. Por ejemplo, el 6 tiene como factores a 1,2 y 3, cuya suma da el número 6. A estos números los llamaron _perfectos._ Escriba un programa que imprima los números menores que un número  $$m$$ dado por el usuario. Verifique probando con $$m =  10000$$. **Sugerencia:** implemente una función que determine los factores de un numero, y otra que verifique si un numero es perfecto o no. Eta ultima función debe devolver un booleano.

**9\)**  El chino Sun Tsu en el año 400 a.c. halló soluciones para el siguiente problema:  
encontrar un entero que al dividirlo por 3, el residuo de 2; al dividirlo por 5, el residuo sea 3, y al dividirlo por 7, el residuo sea 2. Escriba un programa que encuentre los numeros menores que $$m$$ \( donde $$m$$ es dado por el usuario\), que satisfacen estas condiciones

**10\)**  Se tienen pesas no repetidas de $$1,2,4,8,16 \; \text{y}\; 32\, kg$$. con ellas se pueden pesar sacos de arroz hasta de 63kg \( $$63=1+2+4+8+16+32$$ \) que tengan masas en multiplos enteros de 1kg. Es decir, para masas en kg de1, 2, 3, 4, etc. Elabore un prigrama que compruebe esta afirmacion. El programa debe sacar una lista hasta 63, de la siguiente manera:

```text
Pesas           Suma
  1               1
  2               2
  2 1             3
  4               4
  4 1             5
  4 2             6
  4 2 1           7
  . .             . . 
```

O si le gusta un reto mayor, dado un saco con una masa entre 1 y 63 kg \(cualquier pero entero en ese intervalo, por ejemplo 33\), elabore un programa que le diga cuales son las pesas que debe utilizar para pesarlo.

**11\)**  Por definición, la derivada de una función viene dada por:

$$
\dfrac{df(x)}{dx} = \lim_{h \to 0} \dfrac{f(x+h)-f(x)}{h}
$$

la cual puede ser interpretada geometricamente como la pendiente de la recta tangente a la curva $$f(x) $$ en el punto $$x$$ . Esta interpretación y la anterior expresion ayuda a determinar la derivada de una funcion en un punto $$a = b$$ de forma numerica usando el computador. Escribir un algoritmo que calcule la derivada de la función $$f(x) = x^3\sin(x)\log(x)$$ en el punto $$ x=2 $$ y verifique que debe darle algo aproximadamente a: 8.892905028026.

**12\)**  La siguiente expresión sirve para calcular de forma aproximada la derivada numérica de una función si $$h$$ \(tamaño de paso\) es pequeño:

$$
\dfrac{df(x)}{dx} \approx \dfrac{f(x+h)-f(x-h)}{2h}
$$

 Escriba una función en python `diff` que retorne la derivada numérica de una función `f`. Para verificar su funcionamiento, utilice como función a la utilizada en el ejercicio 11: $$f(x) = x^3\sin(x)\log(x)$$, y compare el resultado obtenido por ambos.

**13\)**  En componentes rectangulares, un vector en 3 dimensiones puede ser escrito de la siguiente forma:

$$
\textbf{A} = A_x\textbf{i} + A_y\textbf{j} +A_z\textbf{k}
$$

donde $$A_x , A_y , A_z$$ son las componentes del vector. Con esta representación, la suma\($$\textbf{C} = \textbf{A} + \textbf{B}$$\), la resta\($$\textbf{C} = \textbf{A} - \textbf{B}$$\), el producto escalar \($$\textbf{A} \cdot \textbf{B}$$\) y el producto vectorial \($$\textbf{A} × \textbf{B}$$\) entre dos vectores queda dado de la siguiente forma:

$$
\begin{eqnarray}
\textbf{C} &=& (A_x ± B _x )\textbf{i} + (A_y ± B_y )\textbf{j} + (A_z ± B_z )\textbf{k} \\ 
\textbf{A} \cdot \textbf{B} &=& A_x B_x + A_y B_y + A_z B_z \\
\textbf{A} × \textbf{B} &=& (A_y B_z − A_z B_y )\textbf{i} − (A_x B_z − A_z B_x )\textbf{j} + (A_x B_y − A_y B_x )\textbf{k}
\end{eqnarray}
$$

Escriba un programa en el que dada las componentes rectangulares de dos vectores $$\textbf{A}$$ y $$\textbf{B}$$ , calcule una de estas operaciones especificada por el usuario. El programa debe mostrar un menu donde se puedan escoger las siguientes operaciones: suma, resta, producto producto escalar,producto vectorial y _Todas las operaciones_ y que permita al usuario ingresar las componentes de cada vector. Si el usuario escoge _Todas las operaciones_, el programa debe mostrar en pantalla el resultado de cada una de ellas.

**14\)**  En un tiro parabólico, el _Alcance Máximo_ es la máxima distancia que recorrería el proyectil horizontalmente, si este se lanzara desde el suelo. El alcance máximo puede ser calculado con la siguiente expresión:

$$
R = \dfrac{v_0^2 \sin 2\theta_0}{g}
$$

Elabore un programa en el que dada una velocidad inicial cualquiera, determine para que ángulo se obtiene un alcance máximo en el lanzamiento. Para este ejercicio debe implementar una funcionalidad que calcule el valor máximo de un conjunto de números de una lista y en que ubicacion se encuentra. 

**15\)**  Una forma de aproximar la función $$\ln(1 + x)$$ es mediante la siguiente fórmula:

$$
L(x,n) = \sum_{i=1}^n \dfrac{1}{i}\left(\dfrac{x}{1+x}\right)^i
$$

donde se cumple que $$\ln(1 + x) =\lim\limits_{n \to \infty} L(x, n)$$. Escriba un programa en donde se evaluará la funcion $$L(x, n)$$ para un mismo valor de $$x$$, y para distintos valores de $$n\, (10,50,100,200,1000,...)$$ y se debe mostrar en pantalla el valor de la función $$L(x, n)$$ obtenido, junto con el valor dado por la función real $$\ln(1 + x)$$ \(usando la librerı́a math\) y el error del valor obtenido:   
 $$\mathrm{error} =|L(x, n) − \ln(1 + x)| $$. Verifique que los valores obtenidos se comienzan a asemejar a medida que $$n$$ crece, es decir, el error se hace mas pequeño.

**16\)**  Encontrar el máximo valor de la función $$f (x) = \sin x/x$$ por inspección. Para esto, tome valores de $$x$$ desde $$ -10$$ hasta $$10$$, cada $$0.1$$ y evalúe la función en cada punto. Al final, el programa debe dar el máximo valor obtenido y el valor de $$x$$ donde esto ocurre. ¿Encontró algun inconveniente para resolver este problema?, ¿como cree que puede solucionarse?

**17\)**  La aproximación de Stirling afirma que para n grande se satisface:

$$
\log(n!) = n \log n − n
$$

Empiece con $$n = 10.0$$ y calcule la diferencia porcentual:

$$
\mathrm{diff} = 100.0 \times \dfrac{\log(n!) − [n \log(n) − n]}{\log(n!)}
$$

Aumente el valor de $$n$$ de uno en uno hasta cuando esa diferencia sea menor que el $$5%$$. Escriba los valores de $$n, \log(n), n \log(n) − n$$ y la diferencia porcentual para cada $$n$$

**18\)**  Dada una precisión suministrada por el usuario, determinar el valor de $$\pi$$a partir de la siguiente expresión:

$$
\dfrac{\pi-3}{4} = \dfrac{1}{2\cdot3\cdot4} - \dfrac{1}{4\cdot5\cdot6}  + \dfrac{1}{6\cdot7\cdot8} - \cdots
$$

