# practica3_2022-1
Práctica 3 Laboratorio de Informática 2 2022-1

Resuelva los siguientes ejercicios utilizando Programación Orientada a Objetos en C++

Fecha de entrega: Agosto 22 de 2022

Se debe crear u repositorio con los archivos fuente y de cabecera de la solución. No se aceptan archivos en extensiones queno sean .cpp, .cc, .h o .hpp. Archivos de texto plano (.txt) cuentan como no haber entregado la solución.

Se envía un correo con el asunto LAB_INFO2_20221_PRACTICA3_NOMBRE_ESTUDIANTE, en el correo debe enviar en enlace al repositorio de su solución a los ejercicios de la práctica.

Ejercicios:

1. Desarrolle una sencilla aplicación en la que se tienen las siguientes clases:

-Una clase "ListaDeObjetos" que tiene entre otros un atributo privado que es un arreglo en el que se pueden almacenar objetos de cierta clase "Objeto". Una instancia de la clase "ListaDeObjetos" debe permitir almacenar cualquier cantidad de elementos de la clase "Objeto".

-Cuándo se crea una "ListaDeObjetos" se le debe poder especificar un tamaño inicial a la lista, o tener un tamaño por defecto, o crearla como copia de otra lista de objetos.

-"ListaDeObjetos" debe tener un método para almacenar "Objetos" en el arreglo. Este método debe permitir:
<ul>
<li>Crear un "Objeto" nuevo y agregarlo al arreglo, en este caso solo se especifica la categoría del objeto.</li>
<li>Añadir al arreglo un "Objeto" existente (creado previamente). En este caso se pasa el "Objeto" a la "ListaDeObjetos"</li>
</ul>

-"ListaDeObjetos" debe tener un método para averiguar la cantidad de "Objetos" almacenados en cualquier momento en el arreglo.

-"ListaDeObjetos" debe tener un método para extraer la información de un "Objeto" en una determinada posición (índice) del arreglo. Este método debe verificar que si haya en realidad algo almacenado en dicha posición, en caso contrario debe imprimir un mensaje avisando que en esa posición no hay nada almacenado.

-La clase "Objeto"por tiene los siguientes miembros privados: Un miembro tipo int para un número serial que identifica al objeto
Un miembro tipo std::string para darle una denominación (caegoría) al objeto

-Los objetos de la clase "Objeto" se crean asignandoles una categoría al momento de su creación. El número serial de los "Objetos" se debe asignar internamente (de manera automática) al momento de la creación del objeto y debe ser secuencial.

-La aplicación debe tener un sencillo menú de opciones que permita ejecutar distintas acciones como crear una lista, agregar objetos a la lista, o desplegar información de un objeto individual o de todos los objetos de la lista.

2. Desarrolle una aplicación sencilla de "Agenda de Citas y Compromisos" que tiene las siguientes clases y funcionalidades:

-Una clase "Cita" que tiene los siguientes miembros de clase: Miembros para almacenar de manera individual los nombres de las dos personas que van a reunirse o citarse. Un miembro de clase para almacenar el nombre del lugar donde van a reunirse. Y además un miembro que es un objeto de una clase llamada "Fecha".

-Dicha clase "Fecha" cuenta con miembros privados de tipo entero para el almacenamiento del año, el mes, el día y la hora, y también un método para verificar que la fecha sea correcta, es decir, que no haya meses ayores a 12, que la hora no sea superior a 24 horas ni inferior a 0 horas, que el día no sea cero o menor a cero y que respete el máximo de días de acuerdo con el mes, y que verifique si el año es bisiesto para el caso del mes de febrero. Esta clase tiene una sobrecarga adicional para ese método ya que se debe permitir ingresar el mes en letras o en números.

-Una clase externa (amiga?) "CreadorDeCitas" permite crear objetos de la clase "Cita" y tiene un método que permite crear una cita. Este método recibe como parámetros de entrada todos los datos para almacenar en los miembros del objeto "Cita" (Para crear una cita). Además este método debe ir agregando las citas que se van creando en una lista de citas (la lista puede guardar máximo 10 citas). Dicha lista debe poder ser consultada a través de una método de la clase que permita ver todas las citas o una cita individual en específico.

-Agregue un pequeño menú de opciones que permita crear citas e ir agregandolas a la lista de citas y también visualizar las citas que ya se han agendado.

3. Implementa una clase llamada “Stack”. Recuerda que un Stack o Pila es una estructura de datos que funciona como una pila o memoria LIFO (lo último que se ingresó es lo primero que sale). Como una torre de monedas apiladas, para llegar a la primera moneda (la de la base) de la torre (pila) primero se debe retirar todas las monedas que están encima de esta.

Esta clase debe tener los siguientes métodos:

-Un constructor por defecto que crea un Stack vacío.

-Un constructor parametrizado que permite crear un Stack con una cantidad variable de elementos, desde 1 hasta n elementos, siendo n la capacidad máxima del Stack.

-Un constructor de copia que permite crear un Stack como copia de otro.

-Un método “push” que permite agregar elementos al Stack. Debes validar que el Stack no esté lleno.

-Un método “pop” para extraer el elemento que está en la cima del Stack. Debes validar que el Stack no esté vacío.

-Un método “top” para averiguar el valor del elemento en la cima del Stack, pero sin extraerlo del mismo.

-Un método “empty” para saber si el Stack está vacío.

-Un método “full” para saber si el Stack está lleno.

-Un método “size” para saber cuántos elementos hay almacenados en el stack en cierto momento.

-Una sobrecarga del operador >> para que, con la función cout, se puedan imprimir todos los elementos que hay en el Stack en cierto momento, y en el orden desde la cima hasta la base del Stack.

-El stack debe guardar elementos del tipo de la clase "Objeto" del primer ejercicio.
