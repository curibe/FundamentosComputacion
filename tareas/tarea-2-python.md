---
description: Semestre 2019-I
---

# Tarea 2 - Python

## Condiciones de entrega

Deben subir a classroom un único archivo \(notebook de Google colab\) con cada uno de los puntos. Se puede hacer la tarea en máximo grupos de 3 estudiantes. 

Como observación adicional y basado en los resultados de la tarea anterior, existen herramientas de python que podrían solucionar algunos de los problemas que se están pidiendo que resuelvan. No se permite utilizar este tipo de herramientas sino lo visto en clase.

**Fecha de entrega:** Martes 29 de Octubre de 2019.

## Ejercicios

### Problema 1

Dado un conjunto de datos suministrados por el usuario, mostrar dicho conjunto en orden inverso.

### Problema 2

Dado un conjunto de datos suministrados por el usuario de forma desordenada, organizar dicha secuencia de números de menor a mayor y mostrar en pantalla. Este es un algortimo de _sorting_; para este caso aplique el algoritmo [_quicksort_](http://sorting.at/) 

### Problema 3

Elaborar un programa que calcule aproximadamente la longitud de una circunferencia de radio $$r$$ \(dado por el usuario\) a partir del perímetro de un polígono regular de $$n$$ lados \(dado también por el usuario\) inscrito en la circunferencia. ¿ Cuál es el valor de n para el cual el perímetro del polígono difiere del perímetro real de la circunferencia en un $$1\% $$ ?.  
**Sugerencia:** Tenga en cuenta que un polígono regular tiene lados iguales, ademas el angulo central $$\alpha$$ que subtiende cada lado es igual para todos. Por lo tanto, si un polígono tiene $$N$$ lados, se tiene que:  
  
                                            $$\alpha = \dfrac{2\pi}{N}\; rad= \dfrac{360}{N} \; deg$$    

### Problema 4

Por definición, la derivada de una función viene dada por:

$$
\dfrac{df(x)}{dx} = \lim_{h \to 0} \dfrac{f(x+h)-f(x)}{h}
$$

la cual puede ser interpretada geométricamente como la pendiente de la recta tangente a la curva $$f(x) $$ en el punto $$x$$ . Esta interpretación y la anterior expresión ayuda a determinar la derivada de una función en un punto $$a = b$$ de forma numérica usando el computador. Escribir un algoritmo que calcule la derivada de un funcion `f(x)` cualquiera, que puede/debe ser definida como otra rutina. Probar con la función $$f(x) = x^3\sin(x)\log(x)$$ en el punto $$ x=2 $$ y verifique que debe darle algo aproximadamente a: 8.892905028026.

### Problema 5

En componentes rectangulares, un vector en 3 dimensiones puede ser escrito de la siguiente forma:

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

Escriba un programa en el que dada las componentes rectangulares de dos vectores $$\textbf{A}$$ y $$\textbf{B}$$ , calcule una de estas operaciones especificada por el usuario. El programa debe mostrar un menú donde se puedan escoger las siguientes operaciones: suma, resta, producto producto escalar,producto vectorial y _Todas las operaciones_ y que permita al usuario ingresar las componentes de cada vector. Si el usuario escoge _Todas las operaciones_, el programa debe mostrar en pantalla el resultado de cada una de ellas.

### Problema 6

Los griegos buscaron números que al encontrarle los factores\(excepto el numero mismo\) y sumarlos, dieran el numero original. Por ejemplo, el 6 tiene como factores a 1,2 y 3, cuya suma da el número 6. A estos números los llamaron _perfectos._ Escriba un programa que imprima los números menores que un número  $$m$$ dado por el usuario. Verifique probando con $$m =  10000$$. **Sugerencia:** implemente una función que determine los factores de un numero, y otra que verifique si un numero es perfecto o no. Eta ultima función debe devolver un booleano.

