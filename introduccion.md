# Introducción

## 1. Instalación de python 

La instalación de python y sus respectivas librerías depende del sistema operativo que se vaya a usar

### 1.1 Instalación en Windows

Para usar python en windows, la forma mas común es instalando una distribución de python y R usada en computación científica, conocida como [anaconda](https://www.anaconda.com/). Esta herramienta no solo instala python sino muchas de sus librerias usada para calculo científico, computación científica, análisis de datos e inteligencia artifical. A través de ella se gestiona todas estas herramientas de trabajo asi como la instalación de otras librerias. 

![](.gitbook/assets/image%20%2842%29.png)

También cabe mencionar que esta herramienta trae el IDE \(Integrated development enviroment\) [spyder](https://www.spyder-ide.org/) que permite llevar a cabo cualquier desarrollo en python con las herramientas integradas que trae. 

![spyder IDE](.gitbook/assets/image%20%2844%29.png)

### 1.2 Instalación en Linux

En el caso de linux, python se instala por defecto con el sistema operativo por lo que no es necesaria su instalación.  A diferencia de windows, en linux es necesario instalar las librerías que se requieran de forma separada, ya sea a través el gestor de paquetes o de la linea de comandos, ya que dichas librerias no vienen preinstaladas. Esto requiere que tenga conocimientos o este familiarizado con el sistema operativo.

Asimismo, se puede usar cualquier editor de texto ofrecido por la distribución de Linux usada, para escribir los codigos necesarios. En estos momentos los editores mas populares entre los desarrolladores son: [VSCode](https://code.visualstudio.com/), [Atom](https://atom.io/), [PyCharm](https://www.jetbrains.com/pycharm/), [SublimeText](https://www.sublimetext.com/) entre otros. Aunque al igual que en windows, también se puede instalar python y sus librerías y entornos de desarrollo\(IDE\) con anaconda.

## 2. Usando python en la nube

En este caso, no es necesario la instalación de python en su computador sino que se hace uso del servicio ofrecido en la nube por algunos terceros. Esto ofrece la ventaja de que podrá programar y ejecutar sus programas de python independiente de su sistema operativo y lo que es mejor, como es un servicio en la nube, lo puede hacer desde cualquier computador\(no tiene que ser el personal\). 

En nuestro caso particular se va a hacer uso de uno servicio que ofrece la plataforma de google y que permite mantener sus archivos guardados en su cuenta de google drive. Este servicio es [google colab](https://colab.research.google.com/notebooks/welcome.ipynb), y hace uso de los[ notebooks de jupyter](https://jupyter.org/) para ejecutar no solo código de python sino de otros lenguajes que el kernel de jupyter permita. Cuando se vea mas a fondo la unidad de python, se entendera sobre los notebooks de python.

![notebook de bienvenida de google colab](.gitbook/assets/image%20%2810%29.png)

Para hacer uso de [google colab](https://colab.research.google.com/), necesita autenticarse e ingresar a su cuenta de google con el fin de darle permisos a este servicio de escribir en su drive y mantener sus archivos sincronizados.

Jupyter es una aplicación que se puede instalar en su computador \(viene por defecto con anaconda\) o la puede probar en su navegador; sin embargo, a diferencia de google colab, al ser un servicio de prueba en la nube, no guarda las sesiones o desarrollos.

{% tabs %}
{% tab title="Main Page" %}
![](.gitbook/assets/image%20%2848%29.png)
{% endtab %}

{% tab title="Try in your browser" %}
![](.gitbook/assets/image%20%2819%29.png)
{% endtab %}
{% endtabs %}

