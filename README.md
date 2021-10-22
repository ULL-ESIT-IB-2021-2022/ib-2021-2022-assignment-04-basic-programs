# Práctica 04. Programas simples. Tipos de Datos y Expresiones.

# Factor de ponderación: 5

### Objetivos

Los objetivos de esta práctica son que el alumnado:

* Se familiarice con las herramientas de escitura, edición y compilación de programas sencillos.
* Sea capaz de desarrollar programas simples en C++.
* Conozca el ciclo de desarrollo de un programa de ordenador.
* Se familiarice con los tipos de datos y expresiones aritméticas.

### Rúbrica de evaluacion de esta práctica

Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva) que se tendrán en cuenta a la hora de evaluar esta práctica:

* El alumnado ha de acreditar que es capaz de realizar programas simples en C++ similares a los que se proponen en este documento.
* El alumnado ha de acreditar conocer los conceptos expuestos en el material de referencia de esta práctica.
* Ha de acreditarse que se es capaz de conectarse a la máquina virtual de la asignatura y ejecutar en ella comandos de Linux.
* Ha de acreditar que es capaz de editar ficheros alojados en la VM de la asignatura usando VSC.
* Ha de demostrar que es capaz de modificar, compilar y ejecutar los programas que desarrolle.

### Introducción

La única manera de aprender a programar es programando. 
Por ello, tanto en esta como en gran parte de las prácticas siguientes se persigue que el alumnado ponga en práctica los conocimientos de programación adquiridos mediante programas de complejidad incremental y que requieren de los conocimientos previos para poder ser resueltos de manera adecuada.
Para lograr ese fin, se proponen ejercicios que el alumno debe desarrollar de forma individual y donde la generación de código para resolver los problemas propuestos le servirá para formularse nuevas preguntas y consolidar los conceptos adquiridos.

### Trabajo previo

1. Implemente su primer código en C++. Para ello, cree un fichero `hello_world.cc` en su máquina. El contenido del archivo es el siguiente:
```cpp
#include <iostream>

int main() {
  std::cout << "Hello World!";
  return 0;
}
```
Una vez creado el archivo debe compilarlo para obtener un archivo ejecutable:
```
g++ -std=c++14 -Wall -o hello_world hello_world.cc
```
Esto da lugar a un fichero ejecutable con nombre `hello_world`.

Puede ejecutar ese programa `hello_world` tal como sigue:
```
./hello_world
```
La salida será la siguiente:
```
Hello World!
```
2. Estudie todo el material (vídeos, documentos y ejercicios) del tema [Primeros Programas](http://www.minidosis.org/#/temas/Cpp.PrimerosProgramas) del curso "Introducción a la programación en C++".
3. Estudie con detenimiento el [artículo](http://www.cplusplus.com/doc/tutorial/basic_io/) sobre entrada y salida en C++.
4. Estudie con detenimiento el [artículo](https://www.tutorialspoint.com/cplusplus/cpp_data_types.htm) tipos básicos en C++.

### Ejercicios 

Cree diferentes subdirectorios:
```
../practica04-simple-programs/ej-01-coste-carretera
```
en los que ha de desarrollar cada uno de los ejercicios que se proponen a continuación (cambiando adecuadamente `01-coste-carretera`).
Para cada uno de los programas, edítelo, compílelo y compruebe que produce el resultado deseado.

En el desarrollo de estos programas preste particular atención a los identificadores que utiliza en el código y el formato del mismo.
Comience para ello por estudiar la 
[Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html).
Revise en particular los apartados 
[General Naming Rules](https://google.github.io/styleguide/cppguide.html#General_Naming_Rules),
[File Names](https://google.github.io/styleguide/cppguide.html#File_Names), 
[Variable Names](https://google.github.io/styleguide/cppguide.html#Variable_Names)
y algunos de los subapartados de 
[Formatting](https://google.github.io/styleguide/cppguide.html#Formatting).

1. Escribir un programa en C++ que calcule y muestre el coste de una carretera en función de (i) su longitud y (ii) el coste por metro. El programa solicitará al usuario únicamente la cantidad de metros de longitud que tiene la carretera, mientras que el coste por metro es un valor conocido de 1624 euros.

2. Escribir un programa en C++ que permita determinar el número de [yenes](https://en.wikipedia.org/wiki/Japanese_yen) equivalente a una cierta cantidad de euros. Para ello, el programa solicitará al usuario que indique de cuántos euros dispone. Una vez introducido la cantidad de euros, mostrará los yuanes equivalentes sabiendo que, a 18 de octubre de 2021, un yen es equivalente a 0.0075 euros de acuerdo a 
[Morningstar for Currency and Coinbase for Cryptocurrency](https://www.google.com/intl/en/googlefinance/disclaimer/). 

3. Escribir un programa en C++ que solicite al usuario la cantidad de monedas 1, 5, 20 y 50 céntimos así como los billetes de 5, 10, 20, 50, 100, 200 y 500 que tiene y calcule y muestre la cantidad de dinero de la que dispone. 

4. Escribir un programa en C++ que calcule y muestre la media de 3 calificaciones de alumnos de la asignatura Informática Básica. El programa solicitará al usuario la calificación de cada uno de los 3 alumnos donde cada calificación será un valor numérico entre `0.0` y `10.0`.

5. Escribir un programa en C++ que calcule el área y el perímetro de un cuadrado. El programa solicitará la longitud del lado del cuadrado y luego mostrará en pantalla un mensaje con el perímetro y el área.

6. Escribir un programa en C++ que calcule la distancia entre 2 puntos, `A` y `B` en el espacio cartesiano de 3 dimensiones. Los puntos `A` y `B` tienen 3 coordenadas cada uno. Es decir, 
   * `A = (x_1, y_1, z_1)`
   * `B = (x_2, y_2, z_2)`
   
El usuario introducirá los valores de `x_1`, `y_1`, `z_1`, `x_2`, `y_2`, `z_2`. 
Una vez introducidos los valores el programa calculará y mostrará la distancia entre los puntos, donde la distancia entre A y B viene definida por la siguiente expresión:
`dist(A, B) = sqrt((x2-x1) + (y2-y1) + (z2-z1))`
Para calcular la raíz cuadrada ha de usarse la función `sqrt()`.
En [este tutorial](https://www.programiz.com/cpp-programming/library-function/cmath/sqrt)
tiene información sobre el uso de esta función.
No olvide incluir el fichero `cmath` para poder utilizarla en su código.

En este tipo de enunciados tenga siempre en cuenta que una cosa son los nombres que se utilizan a la hora de enunciar o especificar un problema y otra son los identificadores que una buena programadora ha de utilizar en su código.

<!-- 
La respuesta a los ejercicios planteados debe encontrarse ubicado en el repositorio personal de prácticas del alumno para su consulta por parte del profesorado de la asignatura antes de comenzar la sesión de prácticas.
-->
