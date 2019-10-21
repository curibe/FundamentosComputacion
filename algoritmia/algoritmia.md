---
description: >-
  Introducción general sobre el concepto y los elementos que se deben considerar
  para plantear o escribir un algoritmo
---

# Generalidades

¿Que ocurre cuando le dan una expresión algebraica y le piden factorizarla?, o cuando le dan una ecuación cuadrática y le piden calcular las raíces de la ecuación, o cuando es martes o jueves y sabe que tiene el curso de fundamentos en computación o en la casa le piden que haga una natilla para la familia?. Todas estas preguntas, a pesar de que representan acciones diferentes, tienen algo en comun: _deben seguir un conjunto de pasos para solucionaras_

> En [matemáticas](https://es.wikipedia.org/wiki/Matem%C3%A1ticas), [lógica](https://es.wikipedia.org/wiki/L%C3%B3gica), [ciencias de la computación](https://es.wikipedia.org/wiki/Ciencias_de_la_computaci%C3%B3n) y disciplinas relacionadas, un **algoritmo** \(del latín, _dixit algorithmus_ y este del griego _arithmos_, que significa «número», quizá también con influencia del nombre del matemático persa [Al-Juarismi](https://es.wikipedia.org/wiki/Al-Juarismi)\)​ es un conjunto de instrucciones o reglas definidas y no-ambigüas, ordenadas y finitas que permite, típicamente, solucionar un problema, realizar un cómputo, procesar datos y llevar a cabo otras tareas o actividades.Dados un estado inicial y una entrada, siguiendo los pasos sucesivos se llega a un estado final y se obtiene una solución. Los algoritmos son el objeto de estudio de la **algoritmia**.​
>
> Tomado de Wikipedia: [https://es.wikipedia.org/wiki/Algoritmo](https://es.wikipedia.org/wiki/Algoritmo)

## Definición

No existe una definición única y universal para describir lo que es un algoritmo, sin embargo todas coinciden en lo siguiente:

> Un algoritmo es un conjunto de pasos precisos, definidos y finitos que conducen a la solución de un problema

donde:

* **Precisión**: indica el orden de la realización de cada paso del proceso
* **Definición**: Indica la exactitud  y la consistencia  de los pasos descritos en el proceso. Si el algoritmo se prueba dos veces, en estas dos veces se debe obtener el mismo resultado
* **Finitud:** Indica el número razonable de pasos, los cuales deben apuntar a la finalización del proceso y producir un resultado en un tiempo finito.

Se suele pensar que cualquier conjunto de instrucciones dada paso a paso se puede considerar un algoritmo, sin embargo esto no es cierto. Para que un conjunto de instrucciones se consideren un algoritmo, **debe cumplir las tres características mencionadas anteriormente**.

Por ejemplo:

> 1\) poner aceite en una sartén  
> 2\) encender el fuego  
> 3\) calentar el aceite  
> 4\) coger un huevo  
> 5\) romper la cáscara  
> 6\) verter el contenido del huevo en la sartén  
> 7\) aderezar con sal  
> 8\) esperar a que tenga buen aspecto.
>
> _Tomado de Introducción a la programación con python 3 de Andrés Marzal._

Esta receta, a pesar de ser un conjunto de instrucciones no es completamente definida puesto que no es claro en ciertos aspectos como la temperatura, el tipo de huevo, la cantidad de sal o de aceite, etc. Esto significa que si diferentes personas siguen estas instrucciones, no obtendrán exactamente el mismo resultado. Es posible que uno de ellos obtenga una comida mas salada en comparación con otra, o que la contextura sea diferente ya que emplearon diferentes tiempos de cocción o alguno obtuvo un huevo frito y otro lo obtuvo casi asado. Inclusive, la instrucción 8 es mas un aspecto subjetivo de la persona que este cocinando.

Todos los pasos o instrucciones en un algoritmo deben ser muy precisos, la instrucción debe ser exacta y no se pueden presentar ambigüedades, y se debe poder realizar en un tiempo finito. Muchas veces las instrucciones parecen ser finitas pero alguna de las instrucciones internas pueden terminar ejecutándose por un tiempo indefinido. Se debe procurar a que las instrucciones sean realizables y viables. Asimismo, las instrucciones dentro de un algoritmo deben estar relacionadas con la solución, esto es, no debe llevar instrucciones innecesarias que no aporten a la solución u obtención del resultado final deseado.

## Partes de un Algoritmo

Por lo general, un algoritmo se plantea cuando se quiere resolver u obtener un resultado final a partir de ciertas condiciones. Esto significa que en general un algoritmo presenta las siguientes características:

1. _Puede contener una o varios datos de entrada_ . Así  como una receta necesita de ingredientes, los algoritmos muchas veces requieren de ciertos insumos para poderse obtener el resultado deseado. Cabe aclarar que pueden haber casos particulares en donde no se necesita suministrar una entrada.
2. _Debe mostrar un resultado._ Cuando se escribe un algoritmo, generalmente se hace con el fin de obtener un resultado final. Este resultado cambia acorde al problema que se este resolviendo, en donde se pueden entregar uno o mas datos de salida.
3. _Debe contener un conjunto de pasos finitos, definidos, ordenados y precisos._ Estos pasos son los que permitirán obtener el objetivo final para el cual se está escribiendo o ejecutando el algoritmo.

En nuestro caso nos vamos a centrar en el desarrollo de algoritmos en el ámbito computacional por lo que podemos resumir lo anterior en lo siguiente:

1. **Entrada:** Son los insumos o datos de entrada que se necesitan para resolver el problema
2. **Proceso:** Es el conjunto de pasos o procedimiento que permitirán resolver el problema con base a los datos de entrada
3. **Salida:** Es el resultado final obtenido al aplicar el proceso. Es lo que se quiere obtener con el algoritmo.

Es fundamental e importante que antes de resolver un problema y formular su respectivo algoritmo, identificar estas tres partes importantes puesto que nos dara una visión global de que es lo que se va a resolver. 

## Elementos para la construcción de un algoritmo

Cuando se plantea un algoritmo computacional para resolver un problema en especifico y obtener un resultado, van a existir elementos que la mayoria de las veces van a estar presentes al momento de la construcción de éste. Independiente de cual sea el problema que se vaya a resolver, van a existir estos elementos que son comunes y estándares, e incluso, estos elementos también se definen en un lenguaje de programación. Estos elementos son:

* Comandos
* Operadores
* Datos
* Variables

### Comandos

Un comando comúnmente se entiende como una orden que se le da al computador para realizar una tarea específica. Para ser un poco mas precisos, los comandos son **palabras reservadas** escritas en un lenguaje natural para el usuario \( por lo general son palabras en ingles o abreviaciones de palabras \)que se usan para que éste se comunique con la máquina. Estas palabras internamente se convierten en lenguaje máquina para que el computador las entienda y asi ejecute la acción que corresponde. Esto es, imagine que el computador tiene un diccionario en el cual, por cada de estas palabras, posee un conjunto de ordenes \(programas de bajo nivel, o a nivel de hardware\) que se ejecutan una vez se le escriba esta orden. Por esta razón se consideran reservadas, puesto que se deben usar con un fin específico. Por ejemplo, el comando **printf** en C se usa para mostrar mensajes en pantalla, y por tanto, cada vez que el computador encuentre esta palabra, sabe que debe ejecutar las ordenes o acciones especificas a bajo nivel que hacen que se muestren mensajes en el monitor.

Cabe anotar que aprender un lenguaje de programación, es en realidad aprender como mínimo el conjunto de palabras reservadas de dicho lenguaje para saber como ordenarle al computador. No es lo único que corresponde aprender porque en realidad cada lenguaje tiene su propia sintaxis y forma de escribir, pero la mayoria tienen en común las ordenes asociadas a estos comandos. Por ejemplo, mostrar mensajes en pantalla, leer datos desde el teclado, hacer ciclos o condicionales, entre otros.

En resumen:

* Todos los lenguajes, naturales o computacionales, tienen palabras que denotan una acción.
* Los comandos son acciones que debe interpretar y ejecutar el computador
* Cada comando conserva una sintaxis determinada, i.e una forma de utilizarlo
* Los lenguajes computacionales tienen en su repertorio comandos dirigidos al procesamiento de archivos y datos, entre ellos: inicio, leer, imprimir

Para el caso de algoritmia, se usa el lenguaje natural del programador \(en nuestro caso, el español\) para denotar estas palabras reservadas. Algunas palabras reservadas que usaremos al momento de escribir un algoritmo son las siguientes:

* **Inicio**: empieza un bloque de instrucciones \(selección, algoritmo o rutina\)
* **Fin**: termina un bloque de instrucciones \(algoritmo o rutina\)
* **Entre**: entra un valor desde un dispositivo de entrada
* **Muestre**: muestra un valor en un dispositivo de salida
* **Si**: una condición
* **Sino**: la negación de una condición
* **Para**: estructura de repetición
* **Haga**: acciones a repetirse
* **Mientras**: condición de repetición
* **Repita**: repite "bloque" de instrucciones de una estructura de repetición

A medida que se profundice en la unidad, se entenderá mejor el significado de cada una de estas palabras y que acciones denota

### Operadores

Los operadores son los elementos matemáticos/computacionales que permiten el uso, transformación y establecer relaciones entre los datos que se usan en el algoritmo. Estos operadores se clasifican en

<table>
  <thead>
    <tr>
      <th style="text-align:left">Tipo</th>
      <th style="text-align:left"><b>Descripci&#xF3;n</b>
      </th>
      <th style="text-align:left"><b>Operadores</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>Operadores matem&#xE1;ticos</b>
      </td>
      <td style="text-align:left">
        <p>Se usan para construir</p>
        <p>f&#xF3;rmulas matem&#xE1;ticas</p>
        <p>y as&#xED; modificar</p>
        <p>las variables</p>
      </td>
      <td style="text-align:left">
        <ul>
          <li>+ (suma)</li>
          <li>- (resta)</li>
          <li>* (multiplicaci&#xF3;n)</li>
          <li>/ (division)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Operadores Relacionales</b>
      </td>
      <td style="text-align:left">
        <p>Sirven para expresar</p>
        <p>las condiciones en los</p>
        <p>algoritmos</p>
      </td>
      <td style="text-align:left">
        <ul>
          <li>&gt; (mayor que)</li>
          <li>&lt; (menor que)</li>
          <li>= (igual)</li>
          <li>&gt;= ( mayor igual)</li>
          <li>&lt;= (menor igual)</li>
          <li>!= (diferente)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Operadores L&#xF3;gicos</b>
      </td>
      <td style="text-align:left">
        <p>Se usan para determinar</p>
        <p>si las variables cumplen</p>
        <p>ciertas condiciones y de</p>
        <p>ah&#xED; tomar decisiones</p>
      </td>
      <td style="text-align:left">
        <ul>
          <li><b>AND</b>
          </li>
          <li><b>OR</b>
          </li>
          <li><b>NOT</b>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
**Importante :** en la mayoría de los lenguajes de programación, el operador "**=**" no es el operador de igualdad matemático sino el operador de asignación. El operador relacional "igual" en programación, que equivale al igual matemático,  se escribe como "**==**". 
{% endhint %}

### Datos

Se puede entender a un dato como _un campo que puede convertirse en información._ Para entender esto imagine que le dan el siguiente par de números: 24 y 24; inicialmente para nosotros esos dos números son iguales pero no significan nada en particular. Si reescribimos estos dos números como 24 kg y 24 °C, ya estos dos números, aunque iguales numéricamente, no significan lo mismo ya que el primero denota una masa y el segundo una temperatura. Por tanto, estos dos datos se han convertido o estan suministrando un tipo de información en particular. No significa que en el computador, estos números se puedan escribir con unidades, mas bien, dependiento del algoritmo y de su contexto, estos datos pueden representar cierta información particular.

Los datos simples pueden ser:

* Numéricos \(Reales, enteros\)
* Lógicos \(o booleanos: verdadero o falso, Si o No\)
* Caracter \(char, string - tira de caracteres\)



### Variables

En el contexto matemático, se entiende como variable a un símbolo que representa a un número:

> In [elementary mathematics](https://en.wikipedia.org/wiki/Elementary_mathematics), a **variable** is a symbol, commonly a single letter, that represents a number, called the value of the variable, which is either arbitrary, not fully specified, or unknown.\[ [wikipedia](https://en.wikipedia.org/wiki/Variable_%28mathematics%29) \]

Sin embargo, este concepto es un poco diferente en el ámbito computacional. En ciencias de la computación se entiende a una variable como espacios de memoria \(RAM\) creados para contener valores que de acuerdo a su naturaleza deseen mantenerse \(constantes\) o que puedan cambiar \(variables\).

* Constantes: Es un dato que permanece sin cambios a lo largo de la ejecución del programa. Se usa cuando se necesita que dicho valor permanezca fijo a lo largo de la ejecución del algoritmo 
* Variable: es un dato cuyo valor puede cambiar a lo largo del desarrollo del algoritmo o en el transcurso de la ejecución del programa

![Definici&#xF3;n, caracter&#xED;sticas y operaciones que se hacen con una variable. Imagen tomada de   https://www.101computing.net/variables-terminology/](../.gitbook/assets/image%20%283%29.png)

Como una variable es un espacio en memoria ram, se puede pensar de forma abstracta como una caja la cual tiene un tamaño dependiendo de la información que se vaya a guardar en ella \(en general el tamaño es en bits\), una dirección que define la ubicación y el dato o información \(dato en binario\). Por lo general la dirección es un string que es dificil entender para el programador, por lo que usa un nombre con el que se representa la variable

![](../.gitbook/assets/image%20%2846%29.png)

> In [computer programming](https://en.wikipedia.org/wiki/Computer_programming), a **variable** or **scalar** is a storage location \(identified by a [memory address](https://en.wikipedia.org/wiki/Memory_address)\) paired with an associated [symbolic name](https://en.wikipedia.org/wiki/Symbol) \(an [identifier](https://en.wikipedia.org/wiki/Identifier_%28computer_programming%29)\), which contains some known or unknown quantity of information referred to as a [value](https://en.wikipedia.org/wiki/Value_%28computer_science%29). The variable name is the usual way to [reference](https://en.wikipedia.org/wiki/Reference_%28computer_science%29) the stored value, in addition to referring to the variable itself, depending on the context. This separation of name and content allows the name to be used independently of the exact information it represents. The identifier in computer [source code](https://en.wikipedia.org/wiki/Source_code) can be [bound](https://en.wikipedia.org/wiki/Name_binding) to a [value](https://en.wikipedia.org/wiki/Value_%28computer_science%29) during [run time](https://en.wikipedia.org/wiki/Run_time_%28program_lifecycle_phase%29), and the value of the variable may thus change during the course of [program execution](https://en.wikipedia.org/wiki/Execution_%28computing%29) \[[wikipedia](https://en.wikipedia.org/wiki/Variable_%28computer_science%29)\]



## Representación de algoritmos

Un algoritmo puede tener diferentes representaciones:

* **Seudocódigo:** Es una descripción formal de un algoritmo en un lenguaje estructurado, basado \(por comodidad\) en la lengua nativa de un programador. Contiene un conjunto bien definido de "palabras", reglas de construcción de "instrucciones", símbolos matemáticos y lógicos, entre otros. No hay un estándar. Cada autor usa sus propias reglas. Hay que tener presente la escritura de un seudocódigo es mas estricta puesto que lo que se quiere es que su sintaxis sea lo mas cercana a un codigo real
* **Diagrama de flujo:** Es una representación gráfica del algoritmo en donde se muestra el flujo completo por medio de cajas o símbolos de distintas formas, lo cual representa una accion especifica, las cuales estan conectadas a través de flechas

![](../.gitbook/assets/image%20%2820%29.png)

* **Programa:** Cualquier implementación de un algoritmo en un "lenguaje" que codifica instrucciones que pueda ejecutar un computador. Se puede entender también como la versión de un algoritmo escrita en el "lenguaje que habla" un computador. En general se puede decir que los algoritmos son las recetas que usamos para realizar una tarea en informática. Los algoritmos pueden ser descritos de muchas maneras. Cuando se usa un lenguaje estructurado se dice que están descritos en pseudo código. Si se usa un lenguaje específico entendible por la máquina decimos que están descritos como un programa.
* **Prueba de Escritorio.** Una vez se ha descrito un algoritmo,¿Cómo se prueba?.La prueba de algoritmos y programas es de los retos más difíciles en la programación puesto que toca ponerse en el lugar de quien ejecuta el algoritmo y ejecutarlo todo tal cuál es descrito en él. Una buena prueba es ejecutar el algoritmo de modo que se recorran todos los posibles "caminos" por el diagrama de flujo.

Por lo general, el flujo que se sigue para resolver un problema es el siguiente:

![](../.gitbook/assets/image%20%284%29.png)

Primero se debe plantera el problema, bosquejar como solucionarlo, identificar las entradas y salidas, plantear el algoritmo y luego pasar dicho algoritmo a un lenguaje de programación real para que pueda ser ejecutado en el computador

{% hint style="warning" %}
Cada uno de las representaciones anteriores son independientes \(excepto la ultima\): Se puede escribir el seudocódigo solamente, o el diagrama de flujo o escribir directamente el programa\(esto se suele hacer cuando se gana experiencia\). Sin embargo, durante el desarrollo de esta unidad se  procedera de la siguiente forma cuando se vaya a solucionar un problema

1. Se entenderá que esta pidiendo el problema. Es necesario tomarse su tiempo en leer el enunciado y entenderlo
2. Se determinará _la\(s\) entrada\(s\), el proceso y la salida\(s\)_ del problema
3. Se definirán las variables a usar: su nombre y el tipo de dato que se va a almacenar en ellas
4. Se construye el diagrama de flujo basado en los items anteriores
5. Se escribe el seudocódigo basado en los items anteriores
6. Se hará la prueba de escritorio.

   6.1 Escribir el seudocódigo en python 

Se discutió en clase que se puede implementar dos herramientas: PSeInt que permite redactar seudocódigos y probarlos \(es una herramienta, no un lenguaje de programación\) o tomar el seudocódigo escrito en el paso 5 y escribirlo en python para luego ejecutarlo.
{% endhint %}





