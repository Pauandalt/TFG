# PRÁCTICA DE REDES NEURONALES

Para realizar esta práctica se usará el programa ["A Neuronal Network Playground"](http://playground.tensorflow.org/). 

["A Neuronal Network Playground"](http://playground.tensorflow.org/) es un programa online que emula el comportamiento de una red neuronal ante una serie de variables de entrada, "input variables" y obtiene una representación geométrica de la misma. Este programa tiene como fin acotar una serie de datos en el espacio que les corresponde en el plano. Para ello, el usuario debe hacer uso de los input necesarios así como de las capas de neuronas correspondientes para clasificar **los puntos naranjas en las regiones naranjas y los azules en las regiones azules**.

### Variable de entrada:

Los input de entrada son funciones que emplea el usuario a modo de hiper-plano para clasificar los datos en diferentes regiones. Las variables de entrada vienen definidas en la parte izquierda del programa: 

![alt text](https://github.com/Pauandalt/TFG/blob/master/Programa.PNG)


#### Ejemplos de input:

**Función Lineal:**

X1 y X2 son funciones lineales que actúan a modo de hiper-planos lineales (planos ortogonales al plano de conjunto de soluciones) y que por tanto crean un línea de separación de los resultados recta.

![alt text](https://github.com/Pauandalt/TFG/blob/master/recta_plano.jpg) ![alt text](https://github.com/Pauandalt/TFG/blob/master/X1.PNG)

**Función Cuadrática:**

X1^2 y X2^2 son funciones cuadráticas que actúan a modo de hiper-planos parabólicos (forman paraboloides ortogonales al plano de soluciones) y que por tanto crean un circunferencias de separación de los resultados recta.

![alt text](https://github.com/Pauandalt/TFG/blob/master/paraboloide.png)![alt text](https://github.com/Pauandalt/TFG/blob/master/X1^2.PNG)

**Función hiperbólica:**

La función X1X2 es la función resultante de multiplicar dos funciones lineales formando un conjunto de soluciones hiperbólico que da la opción de dividir en 4 regiones diferentes el plano de resultados de manera inmediata.

![alt text](https://github.com/Pauandalt/TFG/blob/master/hiperbola.png) ![alt text](https://github.com/Pauandalt/TFG/blob/master/X1X2%20plot.PNG)

**Función senoidal:**

La función sin(X1) divide el plano de soluciones en múltiples regiones de manera alterna.

![alt text](https://github.com/Pauandalt/TFG/blob/master/senoidal.jpg) ![alt text](https://github.com/Pauandalt/TFG/blob/master/sinX1.PNG)

### Capas neuronales:

La red neuronal es un sistema formado por una serie de capas que el usuario puede utilizar para ajustar las función de entrada al campo de datos deseado. Para ello, las neuronas modifican la forma de la función de entrada y de esta manera, el programa selecciona la cantidad de deformación que cada neurona ejerce sobre la función para que esta pueda acotar el espacio deseado.

![alt text](https://github.com/Pauandalt/TFG/blob/master/Captura.PNG)

 Cada capa tendrá que incorporar un mínimo de dos neuronas porque incorporar tan solo una sería igual que conectar la variable de entrada a la de salida.

Veamos el siguiente ejemplo:

Queremos acotar una serie de puntos formados de manera circular. Dentro del círculo estarían los puntos azules mientras que fuera tendríamos los puntos naranjas . Introduciendo x1 y x2 como input (función de entrada) tan solo podríamos acotar los puntos de manera lineal y por tanto la solución del problema sería imposible. 

![alt text](https://github.com/Pauandalt/TFG/blob/master/ejemplo%201.PNG)

Si introducimos una capa de tan solo dos neuronas observamos que la línea recta que acota los puntos toma forma curva. Las neuronas “doblan” el hiperplano recto que forman las variables de entrada.

![alt text](https://github.com/Pauandalt/TFG/blob/master/ejemplo%202.PNG)

Introduciendo una neurona más en la capa, el plano se podrá doblar de manera que forme un círculo y por tanto el programa podrá acotar la nube de puntos.

![alt text](https://github.com/Pauandalt/TFG/blob/master/ejemplo%203.PNG)

## PRÁCTICA

### Ejercicio 0:
Pruebe a realizar el ejemplo mencionado anteriormente.

![alt text](https://github.com/Pauandalt/TFG/blob/master/ejercicio%200.PNG)

  a)	¿Qué pasaría al añadir más neuronas a la capa??
  b)	¿Qué número de neuronas acota mejor el espacio de datos?
  c)	Añada una capa más a la red neuronal. En la primera capa coloque 5 neuronas y en la segunda tan solo dos. Ejecute el programa. ¿nota alguna diferencia al sumarle una capa de dos neuronas?
  Ahora intercambien el número de neuronas, establezca 2 en la primera capa y 5 en la segunda, ¿qué podemos observar? 


