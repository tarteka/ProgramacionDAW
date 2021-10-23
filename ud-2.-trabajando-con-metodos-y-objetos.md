# UD 2. Trabajando con métodos y objetos

## 1 Introducción

Si nos paramos a observar el mundo que nos rodea, podemos apreciar que casi todo está formado por **objetos**. Existen coches, edificios, sillas, mesas, semáforos, ascensores e incluso personas o animales. **Todos ellos pueden ser considerados objetos, con una serie de características y comportamientos. **Por ejemplo, existen coches de diferentes marcas, colores, etc. y pueden acelerar, frenar, girar, etc., o las personas tenemos diferente color de pelo, ojos, altura y peso y podemos nacer, crecer, comer, dormir, etc.

Los programas son el resultado de la búsqueda y obtención de una solución para un problema del mundo real. Pero ¿en qué medida los programas están organizados de la misma manera que el problema que tratan de solucionar? La respuesta es que muchas veces los programas se ajustan más a los términos del sistema en el que se ejecutarán que a los del propio problema.

Si redactamos los programas utilizando los mismos términos de nuestro mundo real, es decir, utilizando objetos, y no los términos del sistema o computadora donde se vaya a ejecutar, conseguiremos que éstos sean más legibles y, por tanto, más fáciles de modificar.

Esto es precisamente lo que pretende la** Programación Orientada a Objetos (POO)**, en inglés **OOP (Object Oriented Programming), **establecer una serie de técnicas que permitan trasladar los problemas del mundo real a nuestro sistema informático. Ahora que ya conocemos la sintaxis básica de Java, es el momento de comenzar a utilizar las características orientadas a objetos de este lenguaje, y estudiar los conceptos fundamentales de este modelo de programación.

Para ello, en primer lugar profundizaremos en las características de los métodos y a continuación introduciremos el concepto de objeto. Todavía no vamos a definir objetos propios pero Java dispone de una rica librería de objetos predefinidos como Scanner, String o Math que podemos utilizar en nuestros programas y queremos empezar a usarlos cuanto antes.

## 2 Métodos

En la UD anterior hemos utilizado métodos para agrupar un conjunto de instrucciones que realizan una determinada tarea e identificarlas mediante un nombre. Esto nos ha permitido dividir los problemas en partes más manejables y sencillas de crear y mantener y de este modo además, hemos podido realizar programas más estructurados y comprensibles, y evitar la redundancia de código en nuestras aplicaciones. Para ello, todos los métodos los hemos declarado como `public static void`\`.

En esta UD vamos a profundizar en las características de los métodos que nos permitirán flexibilizar aún más nuestros programas. Aprenderemos a utilizar parámetros en nuestros métodos, de manera que podamos resolver tareas parecidas que dependan de uno o varios datos externos. Para ello, será imprescindible desarrollar nuestra capacidad para generalizar problemas.

A continuación, discutiremos la capacidad de los métodos de devolver valores mediante la sentencia `return` y aprovecharemos la capacidad de los objetos para disponer de sus propios métodos. Estos métodos crean lo que se denomina la interfaz del objeto.

### 2.1 Declaración de un método

La definición de un método se compone de dos partes:

* **Cabecera del método**, que contiene el nombre del método junto con el tipo devuelto, un conjunto de posibles modificadores y una lista de parámetros.
* **Cuerpo del método**, que contiene las sentencias que implementan el comportamiento del método (incluidas posibles sentencias de declaración de variables locales).

Los **elementos mínimos** que deben aparecer en la declaración de un método son:

* El tipo devuelto por el método.
* El nombre del método.
* Los paréntesis.
* El cuerpo del método entre llaves: { }.

Por ejemplo, en la clase `Punto` que se ha estado utilizando en los apartados anteriores podrías encontrar el siguiente método:

```
int obtenerX ()
{
// Cuerpo del método
...
} 
```

Donde:

* El tipo devuelto por el método es `int`.
* El nombre del método es `obtenerX`.
* No recibe ningún parámetro: aparece una lista vacía entre paréntesis: `()`.
* El cuerpo del método es todo el código que habría encerrado entre llaves: `{ }`.

Dentro del cuerpo del método podrás encontrar declaraciones de variables, sentencias y todo tipo de estructuras de control (bucles, condiciones, etc.) que has estudiado en los apartados anteriores.

Ahora bien, la declaración de un método puede incluir algunos elementos más. Vamos a estudiar con detalle cada uno de ellos.

![](.gitbook/assets/PROG02\_CONT\_R25\_Metodos.png)
