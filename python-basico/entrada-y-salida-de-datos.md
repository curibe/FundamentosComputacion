# Entrada y Salida de datos

Uno de los primeros procesos fundamentales en la escritura de un programa es el manejo de las entradas y salidas de los datos, ya que por medio de estos es que el usuario va a suministrar información y obtener información del proceso que este llevando a cabo el computador.

La salida de datos no necesariamente debe ser a través del monitor, sino a través de cualquier periférico del computador como lo es la impresora, la red de internet, parlantes, e incluso al disco duro \(el resultado se guarda en un archivo\)

En este caso veremos como obtener una salida de datos a través del monitor con python

## Comando print

El comando `print` es una función que recibe como argumento el mensaje o información que se quiera mostrar en pantalla:

![](../.gitbook/assets/image%20%2841%29.png)

Por ejemplo, para mostrar un mensaje 

Hay distintas formas de mostrar un mensaje en pantalla con el comando print en python: usando las formas estándares que se emplean en cualquier lenguaje o empleando estilos personalizados del mismo lenguaje. 

### Uso básico

Hay dos formas básicas usadas en python para mostrar un mensaje en pantalla:

![](../.gitbook/assets/image%20%2829%29.png)

{% code title="Forma básica 1" %}
```python
#*****************************
# USO DEL COMANDO PRINT
#*****************************

# 1) Uso basico
#------------------------
print("Hola a todos!!")
```
{% endcode %}

![](../.gitbook/assets/image%20%2833%29.png)

```python
# 1) Uso basico con varios argumentos
#------------------------
print("Hola","a", "todos!!")
```

### Formas estandares

```python
#*****************************
# USO DEL COMANDO PRINT
#*****************************

# 1) Uso basico
#------------------------
print("Hola a todos!!")


# 2) Usando print con variables
# Definiendo variables
var1 = 3
var2 = 5.5
var3 = "tira de caracteres"

print(var1,var2,var3)
print("var1: ",var1, " var2: ", var2,"var3: ",var3)
#usando especificadores
print("Especificadores -- var1: %d  var2: %f  var3: %s"%(var1,var2,var3))

print("Haciendo operaciones: ",var1*var2,3.141592654)

# 3) Usando python 3.x
# Similar a los especificadores.
print("var1:{2} - var2:{1} - var3:{1}".format(var1,var2,var3))

# 4) Usando f-string empleado en python 3.6 en adelante
print(f"var1:{var1}  var2:{var2}  var3:{var3} ")

#5) Usando caracteres especiales

print(""""
Esto es un mensaje
   en mul   ti
                       ples 
		lineas
	en la
pantalla"
""")

print("esto \
	es un mensaje \
	  en varias \
lineas")
```

