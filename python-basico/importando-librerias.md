---
description: >-
  Se aprenderá las distintas formas en como se puede importar una libreria en
  python
---

# Importando librerias

Muchas veces uno tiene un conjunto de funciones o rutinas que pueden ser útiles en alguna situación especifica, por ejemplo: rutinas que hagan operaciones vectorial, que calculen la derivada o la integral numérica, que hagan permutaciones, que resuelvan una ecuacion diferencial, que calcule los elementos orbitales de un sistema, que lean las condiciones iniciales de un problema.

Una de las ventajas de python es que tiene muchas librerías que pueden ser implementadas para nuestros programas \(no toca reinventar la rueda\) y que ya estan optimizadas. Imaginen que python es como la estructura en la cual uds pueden crear su propio juguete, a su gusto.

Unas de las cosas importantes que hay que tener en cuenta es que la forma en como se importan y se unan las librerias en python esta muy asociado a un paradigma de programación conocido como Programación Orientada a Objetos\(POO\). Si ya esta familiarizado con esta forma de programación, comprenderá la forma en como se usan las funciones de la libreria; sin embargo, no significa que sea requisito entender POO para aprender a importar y usar librerias.

Existen distintas formas de importar una libreria en python

### **Forma 1**

```python
# Se importa la libreria "libreria"
import libreria

# Uso de la libreria
libreria.funcion(args...)
```

Por ejemplo, vamos a importar la librería matemática en python:

```python
# Importando libreria math
import math

# Llamando la libreria
print(math.sqrt(2))
print(math.log(5))
```

Note que en este caso, para poder usar una función matemática es necesario colocar primer el nombre de la librería, seguida de un punto y seguido del nombre de la función.

Note que si se intenta llamar a la función por su nombre propio, se genera un error:

![](../.gitbook/assets/image%20%2828%29.png)

Algunas veces estas librerias no solo contienen funciones o constantes sino también sublibrerias que pueden contener funciones, constantes y otra sublibreria, es decir, una subsublibreria de la libreria principal. En ese caso, la forma de importarlo seria la siguiente:



```python
# Se importa la libreria "libreria"
import libreria.sublibreria.subsublibreria

# Uso de la libreria
libreria.sublibreria.subsublibreria.funcion(args...)
```

Por ejemplo, usando la libreria sckit-learn, un ejemplo de este tipo seria:

```python
# Importanto libreria
import sklearn.feature_extraction.text

# Usando libreria
sklearn.feature_extraction.text.numbers(args...)
```

En el siguiente link se puede encontrar las funciones y constantes que contiene la libreria math: [https://docs.python.org/3/library/math.html](https://docs.python.org/3/library/math.html)

| Function | Description |
| :--- | :--- |
| `ceil(x)` | Returns the smallest integer greater than or equal to x. |
| `copysign(x, y)` | Returns x with the sign of y |
| `fabs(x)` | Returns the absolute value of x |
| `factorial(x)` | Returns the factorial of x |
| `floor(x)` | Returns the largest integer less than or equal to x |
| `fmod(x, y)` | Returns the remainder when x is divided by y |
| `frexp(x)` | Returns the mantissa and exponent of x as the pair \(m, e\) |
| `fsum(iterable)` | Returns an accurate floating point sum of values in the iterable |
| `isfinite(x)` | Returns True if x is neither an infinity nor a NaN \(Not a Number\) |
| `isinf(x)` | Returns True if x is a positive or negative infinity |
| `isnan(x)` | Returns True if x is a NaN |
| `ldexp(x, i)` | Returns x \* \(2\*\*i\) |
| `modf(x)` | Returns the fractional and integer parts of x |
| `trunc(x)` | Returns the truncated integer value of x |
| `exp(x)` | Returns e\*\*x |
| `expm1(x)` | Returns e\*\*x - 1 |
| `log(x[, base])` | Returns the logarithm of x to the base \(defaults to e\) |
| `log1p(x)` | Returns the natural logarithm of 1+x |
| `log2(x)` | Returns the base-2 logarithm of x |
| `log10(x)` | Returns the base-10 logarithm of x |
| `pow(x, y)` | Returns x raised to the power y |
| `sqrt(x)` | Returns the square root of x |
| `acos(x)` | Returns the arc cosine of x |
| `asin(x)` | Returns the arc sine of x |
| `atan(x)` | Returns the arc tangent of x |
| `atan2(y, x)` | Returns atan\(y / x\) |
| `cos(x)` | Returns the cosine of x |
| `hypot(x, y)` | Returns the Euclidean norm, sqrt\(x\*x + y\*y\) |
| `sin(x)` | Returns the sine of x |
| `tan(x)` | Returns the tangent of x |
| `degrees(x)` | Converts angle x from radians to degrees |
| `radians(x)` | Converts angle x from degrees to radians |
| `acosh(x)` | Returns the inverse hyperbolic cosine of x |
| `asinh(x)` | Returns the inverse hyperbolic sine of x |
| `atanh(x)` | Returns the inverse hyperbolic tangent of x |
| `cosh(x)` | Returns the hyperbolic cosine of x |
| `sinh(x)` | Returns the hyperbolic cosine of x |
| `tanh(x)` | Returns the hyperbolic tangent of x |
| `erf(x)` | Returns the error function at x |
| `erfc(x)` | Returns the complementary error function at x |
| `gamma(x)` | Returns the Gamma function at x |
| `lgamma(x)` | Returns the natural logarithm of the absolute value of the Gamma function at x |
| `pi` | Mathematical constant, the ratio of circumference of a circle to it's diameter \(3.14159...\) |
| `e` | mathematical constant e \(2.71828...\) |

Tabla tomada de [https://www.programiz.com/python-programming/modules/math](https://www.programiz.com/python-programming/modules/math)

### Forma 2

Otra forma de importar la libreria es usando un nombre corto o acronimo de la libreria:

```python
# Importando libreria pero con un nombre corto
# Note la palabra "as"
import libreria as nombre_corto

# Usando la libreria
nombre_corto.funcion(args...)
```

Para el ejemplo con la libreria math, seria asi:

```python
import math as m

# Forma de llamar una funcion de esta forma
print( m.exp(1) )
```

Note que el nombre corto se usa para evitar escribir el nombre completo de la libreria que se vaya a usar. Hay casos donde el nombre de la libreria es mas largo por lo que se vuelve engorroso estar escribiendo todo el nombre de la librería

Esto es muy utl cuando se usan librerias y sublibrerias. Por ejemplo:

```python
# Importando libreria con acrónimo
import scipy.spatial.distance as spdist

# Usando acrónimo asignado
print(spdist.pdist(args...))
```

Note que en este caso, no tocó escribir todo el nombre completo de la libreria y sublibreria sino el acrónimo.

### Forma 3

Hay que tener en cuenta que cuando se usa la forma 1 y 2, toda la libreria \(sus funciones\) se cargan a la memoria RAM. Hay situaciones donde esto no nos importa pero hay casos donde uno podria querer ser cuidadoso en cuidar el tamaño de la RAM usado. En este caso, la tercera forma de importar la libreria seria no importandola toda sino alguna de sus funciones: 

```python
# Importando algunas funciones de la libreria
# Pueden ser una o varias
from libreria import funcion1, funcion2,...,funcion

"""
Usando la libreria
Note que en este caso no hay que usar el nombre
de la funcion sino que se puede usar el nombre directo
de cada funcion
"""
funcion1(args...)
funcion2(args...)
```

Para el ejemplo con la librería math, esta forma quedaría así:

```python
# Importando la funcion sqrt y exp de la libreria math
from math import sqrt,exp

# Usando las funciones sqrt y exp con su propio nombre
print( sqrt(2) )
print( exp(1) )
```

En este caso sólo se podrá usar las funciones sqrt y exp. Si se intentara usar otra funcion, se generaría error:

![](../.gitbook/assets/image%20%2858%29.png)

Para el caso de librerias y sublibrerias, se puede importar algunas funciones de las sublibrerias:

```python
# Importando algunas funciones de la subsublibreria distance
from scipy.spatial.distance import pdist,seuclidean

# Usando funciones importadas
print( pdist(args....) )
print( seuclidean(args...) )
```

En este curso, no solo se vera el uso de la libreria math sino que tambien se vera el uso de la libreria Numpy, Matplotlib, Scipy\(si da el tiempo\), Pandas \(si da el tiempo\). El esquema de importar la libreria seguiria siendo el mismo, solo hay que tener en cuenta cuales son sun funciones, sublibrerias, etc.

