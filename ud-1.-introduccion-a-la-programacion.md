# UD 1. Introducción a la programación

## 1 Introducción

En esta primera unidad realizaremos una revisión de algunos conceptos básicos relacionados con la programación de ordenadores. Muchos de ellos se desarrollarán más en profundidad en unidades posteriores o en otros módulos, pero se considera interesante hablar de ellos antes de empezar a programar en Java.

A continuación, **comenzaremos nuestra exploración de Java analizando programas simples que permiten mostrar diferentes mensajes por consola**. Ello, nos permitirá conocer los elementos básicos de los programas en Java a través programas con una estructura muy sencilla.

Por último, estudiaremos la técnica de descomposición y aprenderemos cómo dividir un programa en Java en múltiples piezas reutilizables denominados métodos. De esta manera, podremos dividir una tarea compleja en subtareas más pequeñas y fáciles de manejar, y evitar la redundancia en nuestros programas.

## 2 Programas y programación

### 2.1 Buscando una solución

| En la vida real...                                | En programación...                                                                                                                                                       |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Observación de la situación o problema.           | **Análisis del problema:** requiere que el problema sea definido y comprendido claramente para que pueda ser analizado con todo detalle.                                 |
| Pensamos en una o varias posibles soluciones.     | **Diseño o desarrollo de algoritmos:** procedimiento paso a paso para solucionar el problema dado.                                                                       |
| Aplicamos la solución que estimamos más adecuada. | **Resolución del algoritmo elegido en la computadora:** consiste en convertir el algoritmo en programa, ejecutarlo y comprobar que soluciona verdaderamente el problema. |

¿Qué virtudes debería tener nuestra solución?

* **Corrección y eficacia:** si resuelve el problema adecuadamente.
* **Eficiencia:** si lo hace en un tiempo mínimo y con un uso óptimo de los recursos del sistema.

Para conseguirlo, cuando afrontemos la construcción de la solución tendremos que tener en cuenta los siguientes conceptos:

1. **Abstracción:** se trata de realizar un análisis del problema para descomponerlo en problemas más pequeños y de menor complejidad, describiendo cada uno de ellos de manera precisa. **Divide y vencerás,** esta suele ser considerada una filosofía general para resolver problemas y de aquí que su nombre no sólo forme parte del vocabulario informático, sino que también se utiliza en muchos otros ámbitos.
2. **Encapsulación:** consiste en ocultar la información para poder implementarla de diferentes maneras sin que esto influya en el resto de elementos.
3. **Modularidad:** estructuraremos cada parte en módulos independientes, cada uno de ellos tendrá su función correspondiente.

### 2.2 Algoritmos y programas

Después de analizar en detalle el problema a solucionar, hemos de diseñar y desarrollar una solución. Para ello, en muchas ocasiones recurriremos a los algoritmos. Pero, **¿Qué es un algoritmo?**

{% hint style="success" %}
**Algoritmo:** secuencia ordenada de pasos, descrita sin ambigüedades, que conducen a la solución de un problema dado.
{% endhint %}

Los algoritmos son independientes de los lenguajes de programación y de las computadoras donde se ejecutan. Un mismo algoritmo puede ser expresado en diferentes lenguajes de programación y podría ser ejecutado en diferentes dispositivos. Piensa en una receta de cocina, ésta puede ser expresada en castellano, inglés o francés, podría ser cocinada en fogón o vitrocerámica, por un cocinero o más, etc. Pero independientemente de todas estas circunstancias, el plato se preparará siguiendo los mismos pasos.

La diferencia fundamental entre algoritmo y **programa** es que, en el segundo, los pasos que permiten resolver el problema, deben escribirse en un determinado **lenguaje de programación** para que puedan ser ejecutados en el ordenador y así obtener la solución.

**Los lenguajes de programación** son sólo un medio para expresar el algoritmo y el ordenador un procesador para ejecutarlo. El diseño de los algoritmos será una tarea que necesitará de la creatividad y conocimientos de las técnicas de programación. Estilos distintos, de distintos programadores a la hora de obtener la solución del problema, darán lugar a algoritmos diferentes, igualmente válidos.

En esencia, todo problema se puede describir por medio de un algoritmo y las características fundamentales que éstos deben cumplir son:

* Debe ser **preciso** e indicar el orden de realización paso a paso.
* Debe estar **definido**, si se ejecuta dos o más veces, debe obtener el mismo resultado cada vez.
* Debe ser **finito**, debe tener un número finito de pasos.

Pero cuando los problemas son complejos, es necesario descomponer éstos en subproblemas más simples y, a su vez, en otros más pequeños. Estas estrategias reciben el nombre de **diseño descendente** o **diseño modular** (**top-down design**). Este sistema se basa en el lema **divide y vencerás**.

Para representar gráficamente los algoritmos que vamos a diseñar, tenemos a nuestra disposición diferentes herramientas que ayudarán a describir su comportamiento de una forma precisa y genérica, para luego poder codificarlos con el lenguaje que nos interese. Entre otras tenemos:

* **Diagramas de flujo:** Esta técnica utiliza símbolos gráficos para la representación del algoritmo. Suele utilizarse en las fases de análisis.
* **Pseudocódigo:** Esta técnica se basa en el uso de palabras clave en lenguaje natural, **constantes**, **variables**, otros objetos, instrucciones y estructuras de programación que expresan de forma escrita la solución del problema. Es la técnica más utilizada actualmente.
* **Tablas de decisión:** En una tabla son representadas las posibles condiciones del problema con sus respectivas acciones. Suele ser una técnica de apoyo al pseudocódigo cuando existen situaciones condicionales complejas.

{% hint style="info" %}
A continuación te ofrecemos un enlace a un vídeo en el que puedes ver los elementos gráficos fundamentales que se utilizan para la generación de diagramas de flujo. [https://www.youtube.com/watch?v=tMEscFCEP0g](https://www.youtube.com/watch?v=tMEscFCEP0g)
{% endhint %}

### 2.3 Lenguajes de programación

Como hemos visto, en todo el proceso de resolución de un problema mediante la creación de software, después del análisis del problema y del diseño del algoritmo que pueda resolverlo, es necesario traducir éste a un lenguaje que exprese claramente cada uno de los pasos a seguir para su correcta ejecución. Este lenguaje recibe el nombre de lenguaje de programación.

{% hint style="success" %}
**Lenguaje de programación:** Conjunto de reglas sintácticas y semánticas, símbolos y palabras especiales establecidas para la construcción de programas. Es un lenguaje artificial, una construcción mental del ser humano para expresar programas.
{% endhint %}

Hay que tener en cuenta que pueden existir sentencias sintácticamente correctas, pero semánticamente incorrectas. Por ejemplo, _“Un avestruz dio un zarpazo a su cuidador”_ está bien construida sintácticamente, pero es evidente que semánticamente no.

Una característica relevante de los lenguajes de programación es, precisamente, que más de un programador pueda usar un conjunto común de instrucciones que sean comprendidas entre ellos. A través de este conjunto se puede lograr la construcción de un programa de forma colaborativa.

Los lenguajes de programación pueden ser clasificados en función de lo cerca que estén del lenguaje humano o del lenguaje de los computadores. El lenguaje de los computadores son códigos binarios, es decir, secuencias de unos y ceros. Detallaremos seguidamente las características principales de los lenguajes de programación.

#### 2.3.1 Lenguaje máquina

Este es el lenguaje utilizado directamente por el procesador, consta de un conjunto de instrucciones codificadas en binario. Es el sistema de códigos directamente interpretable por un **circuito microprogramable**.

Este fue el primer lenguaje utilizado para la programación de computadores. De hecho, cada máquina tenía su propio conjunto de instrucciones codificadas en ceros y unos. Cuando un algoritmo está escrito en este tipo de lenguaje, decimos que está en código máquina.

Programar en este tipo de lenguaje presentaba los siguientes inconvenientes:

* Cada programa era válido sólo para un tipo de procesador u ordenador.
* La lectura o interpretación de los programas era extremadamente difícil y, por tanto, insertar modificaciones resultaba muy costoso.
* Los programadores de la época debían memorizar largas combinaciones de ceros y unos, que equivalían a las instrucciones disponibles para los diferentes tipos de procesadores.
* Los programadores se encargaban de introducir los códigos binarios en el computador, lo que provocaba largos tiempos de preparación y posibles errores.

A continuación, se muestran algunos códigos binarios equivalentes a las operaciones de suma, resta y movimiento de datos en lenguaje máquina.

| Operación | Lenguaje máquina |
| --------- | ---------------- |
| SUMAR     | 00101101         |
| RESTAR    | 00010011         |
| MOVER     | 00111010         |

Dada la complejidad y dificultades que ofrecía este lenguaje, fue sustituido por otros más sencillos y fáciles utilizar. No obstante, hay que tener en cuenta que todos los programas para poder ser ejecutados, han de traducirse siempre al lenguaje máquina que es el único que entiende la computadora.

#### 2.3.2 Lenguaje Ensamblador

La evolución del lenguaje máquina fue el lenguaje ensamblador. Las instrucciones ya no son secuencias binarias, se sustituyen por códigos de operación que describen una operación elemental del procesador. Es un lenguaje de bajo nivel, al igual que el lenguaje máquina, ya que dependen directamente del hardware donde son ejecutados.

{% hint style="success" %}
**Mnemotécnico:** son palabras especiales, que sustituyen largas secuencias de ceros y unos, utilizadas para referirse a diferentes operaciones disponibles en el juego de instrucciones que soporta cada máquina en particular.
{% endhint %}

En ensamblador, cada instrucción (mnemotécnico) se corresponde a una instrucción del procesador. En la siguiente tabla se muestran algunos ejemplos.

| Operación   | Lenguaje Ensamblador |
| ----------- | -------------------- |
| MULTIPLICAR | MUL                  |
| DIVIDIR     | DIV                  |
| MOVER       | MOV                  |

En el siguiente gráfico puedes ver parte de un programa escrito en lenguaje ensamblador. En color rojo se ha resaltado el código máquina en **hexadecimal**, en magenta el código escrito en ensamblador y en azul, las direcciones de memoria donde se encuentra el código.

![](.gitbook/assets/PROG01\_CONT\_R10\_ensamblador.jpg)

Pero aunque ensamblador fue un intento por aproximar el lenguaje de los procesadores al lenguaje humano, presentaba múltiples dificultades:

* Los programas seguían dependiendo directamente del hardware que los soportaba.
* Los programadores tenían que conocer detalladamente la máquina sobre la que programaban, ya que debían hacer un uso adecuado de los recursos de dichos sistemas.
* La lectura, interpretación o modificación de los programas seguía presentando dificultades.

Todo programa escrito en lenguaje ensamblador necesita de un intermediario, que realice la traducción de cada una de las instrucciones que componen su código al lenguaje máquina correspondiente. Este intermediario es el programa ensamblador. El programa original escrito en lenguaje ensamblador constituye el código fuente y el programa traducido al lenguaje máquina se conoce como programa objeto que será directamente ejecutado por la computadora.

#### 2.3.3 Lenguajes compilados

Para paliar los problemas derivados del uso del lenguaje ensamblador y con el objetivo de acercar la programación hacia el uso de un lenguaje más cercano al humano que al del computador, nacieron los lenguajes compilados. Algunos ejemplos de este tipo de lenguajes son: Pascal, Fortran, Algol, C, **C++**, etc.

Al ser lenguajes más cercanos al humano, también se les denomina **lenguajes de alto nivel**. Son más fáciles de utilizar y comprender, las instrucciones que forman parte de estos lenguajes utilizan palabras y signos reconocibles por el programador.

¿Cuáles son sus **ventajas**?

* Son mucho más fáciles de aprender y de utilizar que sus predecesores.
* Se reduce el tiempo para desarrollar programas, así como los costes.
* Son independientes del hardware, los programas pueden ejecutarse en diferentes tipos de máquina.
* La lectura, interpretación y modificación de los programas es mucho más sencilla.

Pero un programa que está escrito en un lenguaje de alto nivel también tiene que traducirse a un código que pueda utilizar la máquina. Los programas traductores que pueden realizar esta operación se llaman compiladores.

{% hint style="success" %}
**Compilador:** es un programa cuya función consiste en traducir el código fuente de un programa escrito en un lenguaje de alto nivel a lenguaje máquina. Al proceso de traducción se le conoce con el nombre de compilación.
{% endhint %}

Para ilustrar el proceso de compilación de programas te proponemos el siguiente equema:

![Proceso de compilación en varias plataformas](.gitbook/assets/CompilationScheme-Spanish.png)

El compilador realizará la traducción y además informará de los posibles errores. Una vez subsanados, se generará el programa traducido a código máquina, conocido como **código objeto**. Este programa aún no podrá ser ejecutado hasta que no se le añadan los módulos de enlace o bibliotecas, durante el proceso de enlazado. Una vez finalizado el enlazado, se obtiene el **código ejecutable**.

#### 2.3.4 Lenguajes interpretados

Se caracterizan por estar diseñados para que su ejecución se realice a través de un **intérprete**. Cada instrucción escrita en un lenguaje interpretado se analiza, traduce y ejecuta tras haber sido verificada. Una vez realizado el proceso por el intérprete, la instrucción se ejecuta, pero no se guarda en memoria.

{% hint style="success" %}
**Intérprete:** es un programa traductor de un lenguaje de alto nivel en el que el proceso de traducción y de ejecución se llevan a cabo simultáneamente, es decir, la instrucción se pasa a lenguaje máquina y se ejecuta directamente. No se genera programa objeto, ni programa ejecutable.
{% endhint %}

Los lenguajes interpretados generan programas de menor tamaño que los generados por un compilador, al no guardar el programa traducido a código máquina. Pero presentan el inconveniente de ser algo más lentos, ya que han de ser traducidos durante su ejecución. Por otra parte, necesitan disponer en la máquina del programa intérprete ejecutándose, algo que no es necesario en el caso de un programa compilado, para los que sólo es necesario tener el programa ejecutable para poder utilizarlo.

Ejemplos de lenguajes interpretados son: **Perl, PHP, Python, JavaScript,** etc.

A medio camino entre los lenguajes compilados y los interpretados, existen los lenguajes que podemos denominar **pseudo-compilados o pseudo-interpretados**, es el caso del **Lenguaje Java**. Java puede verse como compilado e interpretado a la vez, ya que su código fuente se compila para obtener el código binario en forma de bytecodes, que son estructuras parecidas a las instrucciones máquina, con la importante propiedad de no ser dependientes de ningún tipo de máquina (se detallarán más adelante). La Máquina Virtual Java se encargará de interpretar este código y, para su ejecución, lo traducirá a código máquina del procesador en particular sobre el que se esté trabajando.

### 2.4 El lenguaje de programación Java

#### 2.4.1 ¿Qué y cómo es Java?

Java es un lenguaje sencillo de aprender, con una sintaxis parecida a la de C++, pero en la que se han eliminado elementos complicados y que pueden originar errores. Java es orientado a objetos, con lo que elimina muchas preocupaciones al programador y permite la utilización de gran cantidad de bibliotecas ya definidas, evitando reescribir código que ya existe. Es un lenguaje de programación creado para satisfacer nuevas necesidades que los lenguajes existentes hasta el momento no eran capaces de solventar.

Una de las principales virtudes de Java es su independencia del hardware, ya que el código que se genera es válido para cualquier plataforma. Este código será ejecutado sobre una máquina virtual denominada **Maquina Virtual Java** (MVJ o JVM – Java Virtual Machine), que interpretará el código convirtiéndolo a código específico de la plataforma que lo soporta. De este modo el programa se escribe una única vez y puede hacerse funcionar en cualquier lugar. Lema del lenguaje: _**“Write once, run everywhere”.**_

Antes de que apareciera Java, el lenguaje C era uno de los más extendidos por su versatilidad. Pero cuando los programas escritos en C aumentaban de volumen, su manejo comenzaba a complicarse. Mediante las técnicas de programación estructurada y programación modular se conseguían reducir estas complicaciones, pero no era suficiente.

Fue entonces cuando la Programación Orientada a Objetos (POO) entra en escena, aproximando notablemente la construcción de programas al pensamiento humano y haciendo más sencillo todo el proceso. Los problemas se dividen en objetos que tienen propiedades e interactúan con otros objetos, de este modo, el programador puede centrarse en cada objeto para programar internamente los elementos y funciones que lo componen.

Las características principales de lenguaje Java se resumen a continuación:

* El código generado por el compilador Java es independiente de la arquitectura.
* Está totalmente orientado a objetos.
* Su sintaxis es similar a C y C++.
* Es distribuido, preparado para aplicaciones **TCP/IP**.
* Dispone de un amplio conjunto de bibliotecas.
* Es robusto, realizando comprobaciones del código en tiempo de compilación y de ejecución.
* La seguridad está garantizada, ya que las aplicaciones Java no acceden a zonas delicadas de memoria o de sistema.

{% hint style="info" %}
Obtén una descripción detallada de las características reseñadas anteriormente a través del siguiente artículo: [Características detalladas del lenguaje Java](http://es.wikibooks.org/wiki/Programaci%C3%B3n\_en\_Java/Caracter%C3%ADsticas\_del\_lenguaje)
{% endhint %}

#### 2.4.1 Breve historia

Java surgió en 1991 cuando un grupo de ingenieros de Sun Microsystems trataron de diseñar un nuevo lenguaje de programación destinado a programar pequeños dispositivos electrónicos. La dificultad de estos dispositivos es que cambian continuamente y para que un programa funcione en el siguiente dispositivo aparecido, hay que rescribir el código. Por eso la empresa Sun quería crear un lenguaje **independiente del dispositivo.**

Pero no fue hasta 1995 cuando pasó a llamarse **Java**, dándose a conocer al público como lenguaje de programación para computadores. Java pasa a ser un lenguaje totalmente independiente de la plataforma y a la vez potente y orientado a objetos. Esa filosofía y su facilidad para crear aplicaciones para redes TCP/IP ha hecho que sea uno de los lenguajes más utilizados en la actualidad.

El factor determinante para su expansión fue la incorporación de un intérprete Java en la versión 2.0 del navegador Web Netscape Navigator, lo que supuso una gran revuelo en Internet. A principios de 1997 apareció **Java 1.1** que proporcionó sustanciales mejoras al lenguaje. **Java 1.2**, más tarde rebautizado como **Java 2,** nació a finales de 1998.

El principal objetivo del lenguaje Java es llegar a ser el **nexo universal** que conecte a los usuarios con la información, esté ésta situada en el ordenador local, en un servidor Web, en una base de datos o en cualquier otro lugar.

Para el desarrollo de programas en lenguaje Java es necesario utilizar un entorno de desarrollo denominado **JDK** (Java Development Kit), que provee de un compilador y un entorno de ejecución (**JRE** – Java Run Environment) para los bytecodes generados a partir del código fuente. Al igual que las diferentes versiones del lenguaje han incorporado mejoras, el entorno de desarrollo y ejecución también ha sido mejorado sucesivamente.

**Java 2** es la tercera versión del lenguaje, pero es algo más que un lenguaje de programación, incluye los siguientes elementos:

* Un lenguaje de programación: Java.
* Un conjunto de bibliotecas estándar que vienen incluidas en la plataforma y que son necesarias en todo entorno Java. Es el Java Core.
* Un conjunto de herramientas para el desarrollo de programas, como es el compilador de bytecodes, el generador de documentación, un depurador, etc.
* Un entorno de ejecución que en definitiva es una máquina virtual que ejecuta los programas traducidos a bytecodes.

El siguiente esquema muestra los elementos fundamentales de la plataforma de desarrollo Java 2.

![](.gitbook/assets/PROG01\_CONT\_R13\_elementos\_plataforma\_java2.png)

Actualmente hay tres ediciones de la plataforma Java 2:

* **J2SE**: Entorno de Sun relacionado con la creación de aplicaciones y **applets** en lenguaje Java.
* **J2EE**: Pensada para la creación de aplicaciones Java empresariales y del lado del servidor.
* **J2ME**: Pensada para la creación de aplicaciones Java para dispositivos móviles.

{% hint style="info" %}
Si deseas conocer más sobre los orígenes del lenguaje Java, aquí te ofrecemos más información:

* [Historia de Java](http://es.wikipedia.org/wiki/Java\_\(lenguaje\_de\_programaci%C3%B3n\)#Historia)
* [Línea de tiempo de la historia de Java](https://www.timetoast.com/timelines/evolution-of-the-smart-car)
{% endhint %}

#### 2.4.3 Independencia de la plataforma y trabajo en red

Existen dos características que distinguen a **Java** de otros lenguajes, como son la **independencia de la plataforma** y la posibilidad de trabajar en red o, mejor, la posibilidad de **crear aplicaciones que trabajan en red**.

Estas características las vamos a explicar a continuación:

1.  **Independencia:** Los programas escritos en Java pueden ser ejecutados en cualquier tipo de hardware. El código fuente es compilado, generándose el código conocido como **Java Bytecode** (instrucciones máquina simplificadas que son específicas de la plataforma Java), el bytecode será interpretado y ejecutado en la **Máquina Virtual** **Java (MVJ o JVM – Java Virtual Machine)** que es un programa escrito en código nativo de la plataforma destino entendible por el hardware. Con esto se evita tener que realizar un programa diferente para cada CPU o plataforma.

    Por tanto, la parte que realmente es dependiente del sistema es la Máquina Virtual Java, así como las librerías o bibliotecas básicas que permiten acceder directamente al hardware de la máquina.
2. **Trabajo en red:** Esta capacidad del lenguaje ofrece múltiples posibilidades para la comunicación vía TCP/IP. Para poder hacerlo existen librerías que permiten el acceso y la interacción con protocolos como **http**, **ftp**, etc., facilitando al programador las tareas del tratamiento de la información a través de redes.

#### 2.4.4 Seguridad y simplicidad

Junto a las características diferenciadoras del lenguaje Java relacionadas con la independencia y el trabajo en red, han de destacarse dos virtudes que hacen a este lenguaje uno de los más extendidos entre la comunidad de programadores: su seguridad y su simplicidad.

1.  **Seguridad:** En primer lugar, los posibles accesos a zonas de memoria “sensibles” que en otros lenguajes como C y C++ podían suponer peligros importantes, se han eliminado en Java.

    En segundo lugar, el código Java es comprobado y verificado para evitar que determinadas secciones del código produzcan efectos no deseados. Los test que se aplican garantizan que las operaciones, operandos, conversiones, uso de clases y demás acciones son seguras.

    Y en tercer lugar, Java no permite la apertura de ficheros en la máquina local, tampoco permite ejecutar ninguna aplicación nativa de una plataforma e impide que se utilicen otros ordenadores como puente, es decir, nadie puede utilizar nuestra máquina para hacer peticiones o realizar operaciones con otra.

    En definitiva, podemos afirmar que Java es un lenguaje seguro.
2.  **Simplicidad:** Aunque Java es tan potente como C o C++, es bastante más sencillo. Posee una curva de aprendizaje muy rápida y, para alguien que comienza a programar en este lenguaje, le resulta relativamente fácil comenzar a escribir aplicaciones interesantes.

    Si has programado alguna vez en C o C++ encontrarás que Java te pone las cosas más fáciles, ya que se han eliminado: la aritmética de **punteros**, los registros, la definición de tipos, la gestión de memoria, etc. Con esta simplificación se reduce bastante la posibilidad de cometer errores comunes en los programas. Un programador experimentado en C o C++ puede cambiar a este lenguaje rápidamente y obtener resultados en muy poco espacio de tiempo.

    Muy relacionado con la simplicidad que aporta Java está la incorporación de un elemento muy útil como es el **Recolector de Basura (Garbage collector)**. Permite al programador liberarse de la gestión de la memoria y hace que ciertos bloques de memoria puedan reaprovecharse, disminuyendo el número de huecos libres (**fragmentación de memoria**).

    Cuando realicemos programas, crearemos objetos, haremos que éstos interaccionen, etc. Todas estas operaciones requieren de uso de memoria del sistema, pero la gestión de ésta será realizada de manera transparente al programador. Todo lo contrario que ocurría en otros lenguajes. Podremos crear tantos objetos como solicitemos, pero nunca tendremos que destruirlos. El entorno de Java borrará los objetos cuando determine que no se van a utilizar más. Este proceso es conocido como recolección de basura.

#### 2.4.5 Java y los Bytecodes

Un programa escrito en Java no es directamente ejecutable, es necesario que el código fuente sea interpretado por la Maquina Virtual Java. ¿Cuáles son los pasos que se siguen desde que se genera el código fuente hasta que se ejecuta? A continuación se detallan cada uno de ellos.

![](.gitbook/assets/PROG01\_CONT\_R16\_programas\_en\_Java.png)

Una vez escrito el código fuente (archivos con extensión `.Java`), éste es precompilado generándose los códigos de bytes, Bytecodes o Java Bytecodes (archivos con extensión `.class`) que serán interpretados directamente por la Maquina Virtual Java y traducidos a código nativo de la plataforma sobre la que se esté ejecutando el programa.&#x20;

{% hint style="success" %}
**Bytecode:** Son un conjunto de instrucciones en lenguaje máquina que no son específicas a ningún procesador o sistema de cómputo. Un intérprete de código de bytes ( bytecodes ) para una plataforma específica será quien los ejecute. A estos intérpretes también se les conoce como Máquinas Virtuales Java o intérpretes Java de tiempo de ejecución.
{% endhint %}

En el proceso de precompilación, existe un verificador de códigos de bytes que se asegurará de que se cumplen las siguientes condiciones:

* El código satisface las especificaciones de la Máquina Virtual Java.
* No existe amenaza contra la integridad del sistema.
* No se producen desbordamientos de memoria.
* Los parámetros y sus tipos son adecuados.
* No existen conversiones de datos no permitidas.

Para que un bytecode pueda ser ejecutado en cualquier plataforma, es imprescindible que dicha plataforma cuente con el intérprete adecuado, es decir, la máquina virtual específica para esa plataforma. En general, la Máquina Virtual Java es un programa de reducido tamaño y gratuito para todos los sistemas operativos.

![](.gitbook/assets/PROG01\_CONT\_R17\_javabytecode.png)

#### 2.4.6 Tipo de aplicaciones en Java

La versatilidad del lenguaje de programación Java permite al programador crear distintos tipos de aplicaciones. A continuación, describiremos las características más relevantes de cada uno de ellos:

* **Aplicaciones de consola:**
  * Son programas independientes al igual que los creados con los lenguajes tradicionales.
  * Se componen como mínimo de un archivo `.class` que debe contar necesariamente con el método `main`.
  * No necesitan un navegador web y se ejecutan cuando invocamos el comando Java para iniciar la Máquina Virtual de Java (JVM). De no encontrarse el método `main` la aplicación no podrá ejecutarse.
  * Las aplicaciones de consola leen y escriben hacia y desde la entrada y salida estándar, sin ninguna interfaz gráfica de usuario.
* **Aplicaciones gráficas:**
  * Aquellas que utilizan las clases con capacidades gráficas, como Swing que es la biblioteca para la interfaz gráfica de usuario avanzada de la plataforma Java SE.
  * Incluyen las instrucciones `import`, que indican al compilador de Java que las clases del paquete `Javax.swing` se incluyan en la compilación.
* **Applets:**
  * Son programas incrustados en otras aplicaciones, normalmente una página web que se muestra en un navegador. Cuando el navegador carga una web que contiene un applet, éste se descarga en el navegador web y comienza a ejecutarse. Esto nos permite crear programas que cualquier usuario puede ejecutar con tan solo cargar la página web en su navegador.
  * Se pueden descargar de Internet y se observan en un navegador. Los applets se descargan junto con una página HTML desde un servidor web y se ejecutan en la máquina cliente.
  * No tienen acceso a partes sensibles (por ejemplo: no pueden escribir archivos), a menos que uno mismo le dé los permisos necesarios en el sistema.
  * No tienen un método principal.
  * Son multiplataforma y pueden ejecutarse en cualquier navegador que soporte Java.
* **Servlets:**
  * Son componentes de la parte del servidor de Java EE, encargados de generar respuestas a las peticiones recibidas de los clientes.
  * Los servlets, al contrario de los applets, son programas que están pensados para trabajar en el lado del servidor y desarrollar aplicaciones Web que interactúen con los clientes.
* **Midlets:**
  * Son aplicaciones creadas en Java para su ejecución en sistemas de propósito simple o dispositivos móviles. Los juegos Java creados para teléfonos móviles son midlets.
  * Son programas creados para dispositivos embebidos (se dedican a una sola actividad), más específicamente para la máquina virtual Java MicroEdition (Java ME).
  * Generalmente son juegos y aplicaciones que se ejecutan en teléfonos móviles.

## 3 Entornos Integrados de Desarrollo (IDE)

En los comienzos de Java la utilización de la línea de comandos era algo habitual. El programador escribía el código fuente empleando un editor de texto básico, seguidamente, pasaba a utilizar un compilador y con él obtenía el código compilado. En un paso posterior, necesitaba emplear una tercera herramienta para el ensamblado del programa. Por último, podía probar a través de la línea de comandos el archivo ejecutable. El problema surgía cuando se producía algún error, lo que provocaba tener que volver a iniciar el proceso completo.

Estas circunstancias hacían que el desarrollo de software no estuviera optimizado. Con el paso del tiempo, se fueron desarrollando aplicaciones que incluían las herramientas necesarias para realizar todo el proceso de programación de forma más sencilla, fiable y rápida. Para cada lenguaje de programación existen múltiples entornos de desarrollo, cada uno con sus ventajas e inconvenientes. Dependiendo de las necesidades de la persona que va a programar, la facilidad de uso o lo agradable que le resulte trabajar con él, se elegirá entre unos u otros entornos.

### 3.1 ¿Qué son?

Son aplicaciones que ofrecen la posibilidad de llevar a cabo el proceso completo de desarrollo de software a través de un único programa. Podremos realizar las labores de edición, compilación, depuración, detección de errores, corrección y ejecución de programas escritos en Java o en otros lenguajes de programación, bajo un entorno gráfico (no mediante línea de comandos). Junto a las capacidades descritas, cada entorno añade otras que ayudan a realizar el proceso de programación, como por ejemplo: código fuente coloreado, plantillas para diferentes tipos de aplicaciones, creación de proyectos, etc.

Hay que tener en cuenta que un entorno de desarrollo no es más que una fachada para el proceso de compilación y ejecución de un programa. ¿Qué quiere decir eso? Pues que si tenemos instalado un IDE y no tenemos instalado el compilador, no tenemos nada.

### **3.2 IDE's actuales**

Existen en el mercado multitud de entornos de desarrollo para el lenguaje Java, los hay de libre distribución, de pago, para principiantes, para profesionales, que consumen más recursos, que son más ligeros, más amigables, más complejos que otros, etc.

Entre los que son gratuitos o de libre distribución tenemos:

* **NetBeans**
* **Eclipse**
* **BlueJ**
* **jGRASP**
* **Jcreator LE**

Entre los que son propietarios o de pago tenemos:

* **IntelliJ IDEA**
* **Jbuilder**
* **Jcreator**
* **JDeveloper**

![Comparativa entornos para Java](.gitbook/assets/comparativa-ides-java.PNG)

Pero, ¿cuál o cuáles son los más utilizados por la comunidad de programadores Java? El puesto de honor se lo disputan entre **Eclipse, NetBeans** y IntelliJ IDEA. Los dos primeros son gratuitos, con soporte de idiomas y multiplataforma (Windows, Linux, MacOS).

¿Y cuál será con el que vamos a trabajar? Pues aunque parezca mentira, ninguno de ellos. Vamos a utilizar [**jGRASP**](http://www.jgrasp.org/index.html) , un entorno de desarrollo ligero, creado por la Universidad de Auburn para mejorar la comprensión del software y facilitar el aprendizaje de la programación. Está desarrollado en Java y funciona con Windows, Linux y MacOS sobre máquinas virtuales de Java.

### **3.3 El entorno jGRASP**

jGRASP es un entorno de desarrollo ligero que ha sido específicamente creado para proporcionar herramientas de visualización de software que facilitan la conprensión del código a programadores principiantes.

En concreto proporciona 3 herramientas principales de visualización:

* Diagramas de estructuras de control para visualización de código fuente
* Diagramas de clases UML para visualizar la arquitectura de proyectos
* Visor de datos primitivos y objetos en tiempo de ejecución

Así mismo, incluye un entorno de trabajo innovador, un debugger y la ventana "Interactions" que nos permite probar código sin crear un programa completo.

Ha sido desarrollado en Java por la Universidad de Auburn, por lo que funciona en cualquier plataforma que tenga la máquina virtual de Java instalada. La página oficial de Java proporciona descargas para Windows, Mac OS y Linux.

Soporta Java, C, C++, Objective-C, Python, Ada, y VHDL. Por ello, no es un IDE profesional sino un IDE pensado para estudiantes que están aprendiendo a programar. La mayoría de sus funcionalidad se orientan a facilitar la comprensión del funcionamiento del código y no a facilitar la generación de código.

## 4. Mi primer programa en Java

Hasta ahora, hemos descrito el lenguaje de programación Java, hemos hecho un recorrido por su historia y nos hemos instruido sobre su filosofía de trabajo, pero te preguntarás ¿Cuándo empezamos a desarrollar programas? ¿Qué elementos forman parte de un programa en Java? ¿Qué se necesita para programar en este lenguaje? ¿Podemos crear programas de diferente tipo?

No te impacientes, cada vez estamos más cerca de comenzar la experiencia con el lenguaje de programación Java. Iniciaremos nuestro camino conociendo cuales son los elementos básicos de un programa Java, la forma en que debemos escribir el código y los tipos de aplicaciones que pueden crearse en este lenguaje.

### 4.1 Estructura básica de un programa

En el gráfico al que puedes acceder a continuación, se presenta la estructura general de un programa realizado en un lenguaje orientado a objetos como es Java.

![](.gitbook/assets/PROG01\_CONT\_R19\_estructura\_programa\_java.jpg)

Vamos a analizar cada uno de los elementos que aparecen en dicho gráfico:

* **public class Clase\_Principal**: Todos los programas han de incluir una clase como esta. Es una clase general en la que se incluyen todos los demás elementos del programa. Entre otras cosas, contiene el método o función `main()` que representa al programa principal, desde el que se llevará a cabo la ejecución del programa. Esta clase puede contener a su vez otras clases del usuario, pero sólo una puede ser `public`. El nombre del fichero `.Java` que contiene el código fuente de nuestro programa, coincidirá con el nombre de la clase que estamos describiendo en estas líneas.
* **public static void main (String\[] args)**: Es el método que representa al programa principal, en él se podrán incluir las instrucciones que estimemos oportunas para la ejecución del programa. Desde él se podrá hacer uso del resto de clases creadas. Todos los programas Java tienen un método `main`.
* **Comentarios**: los comentarios se suelen incluir en el código fuente para realizar aclaraciones, anotaciones o cualquier otra indicación que el programador estime oportuna. Estos comentarios pueden introducirse de dos formas, **con** `//` y **con** `/* */`. Con la primera forma estaríamos estableciendo una única línea completa de comentario y, con la segunda, con `/*` comenzaríamos el comentario y éste no terminaría hasta que no insertáramos `*/`.
* **Bloques de código**: son conjuntos de instrucciones que se marcan mediante la apertura y cierre de llaves `{ }`. El código así marcado es considerado interno al bloque.
* **Punto y coma**: aunque en el ejemplo no hemos incluido ninguna línea de código que termine con punto y coma, hay que hacer hincapié en que cada línea de código ha de terminar con punto y coma (`;`). En caso de no hacerlo, tendremos errores sintácticos. _\*\*_

{% hint style="danger" %}
Ten en cuenta que **Java distingue entre mayúsculas y minúsculas**. Si le das a la clase principal el nombre PrimerPrograma, el archivo **`.java`** tendrá como identificador **PrimerPrograma.java**, que es totalmente diferente a primerprograma.Java. Además, para Java los elementos PrimerPrograma y primerprograma serían considerados dos clases diferentes dentro del código fuente.
{% endhint %}

### 4.2 Identificadores

Como hemos visto en un programa vamos a encontrar clases y métodos a los que tendremos que dar un nombre lo más representativo posible para que nos ayude a entender el programa. Al nombre que le damos se le llama **identificador**.

Los identificadores permiten nombrar los elementos que se están manejando en un programa. Vamos a ver con más detalle ciertos aspectos sobre los identificadores que debemos tener en cuenta.

#### 4.2.1 Identificadores

Un **identificador** en Java es una secuencia ilimitada sin espacios de letras y dígitos **Unicode**, de forma que **el primer símbolo de la secuencia debe ser una letra, un símbolo de subrayado (\_) o el símbolo dólar ($)**. Por ejemplo, son válidos los siguientes identificadores:

```
$x5      ατη    NUM_MAX    _numCuenta
```

En la definición anterior decimos que un identificador es una secuencia ilimitada de caracteres Unicode. Pero… ¿qué es Unicode? Unicode es un código de caracteres o sistema de codificación, un alfabeto que recoge los caracteres de prácticamente todos los idiomas importantes del mundo. Las líneas de código en los programas se escriben usando ese conjunto de caracteres Unicode.

Esto quiere decir que en Java se pueden utilizar varios alfabetos como el Griego, Árabe o Japonés. De esta forma, los programas están más adaptados a los lenguajes e idiomas locales, por lo que son más significativos y fáciles de entender tanto para los programadores que escriben el código, como para los que posteriormente lo tienen que interpretar, para introducir alguna nueva funcionalidad o modificación en la aplicación.

El estándar Unicode originalmente utilizaba 16 bits, pudiendo representar hasta 65.536 caracteres distintos, que es el resultado de elevar dos a la potencia dieciséis. Actualmente Unicode puede utilizar más o menos bits, dependiendo del formato que se utilice: **UTF-8**, **UTF-16** ó **UTF-32. A cada carácter le corresponde unívocamente un número entero perteneciente al intervalo de 0 a 2 elevado a n, siendo n el número de bits utilizados para representar los caracteres. Por ejemplo, la letra** ñ es el entero 164. Además, el código Unicode es “compatible” con el código ASCII, ya que para los caracteres del código ASCII, Unicode asigna como código los mismos 8 bits, a los que les añade a la izquierda otros 8 bits todos a cero. La conversión de un carácter ASCII a Unicode es inmediata.

{% hint style="warning" %}
Una buena práctica de programación es seleccionar nombres adecuados para las variables, eso ayuda a que el programa se autodocumente, y evita un número excesivo de comentarios para aclarar el código.
{% endhint %}

#### 4.2.2 Convenios y reglas para nombrar variables

A la hora de nombrar un identificador existen una serie de normas de estilo de uso generalizado que, no siendo obligatorias, se usan en la mayor parte del código Java. Estas reglas para la nomenclatura de variables son las siguientes:

* **Java distingue las mayúsculas de las minúsculas**. Por ejemplo, `Alumno` y `alumno` son variables diferentes.
* **No se suelen utilizar identificadores que comiencen con «$» o «\_»,** además el símbolo del dólar, por convenio, no se utiliza nunca.
* **No se puede utilizar el valor booleano** (`true` o `false`) **ni el valor nulo** (`null`).
* Los **identificadores deben ser lo más descriptivos posibles**. Es mejor usar palabras completas en vez de abreviaturas crípticas. Así nuestro código será más fácil de leer y comprender. En muchos casos también hará que nuestro código se autodocumente. Por ejemplo, si tenemos que darle el nombre a una variable que almacena los datos de un cliente sería recomendable que la misma se llamara algo así como `FicheroClientes` o `ManejadorCliente`, y no algo poco descriptivo como `Cl33`.

Además de estas restricciones, en la siguiente tabla puedes ver otras convenciones, que no siendo obligatorias, sí son recomendables a la hora de crear identificadores en Java.

| Identificador | Convención                                                                                                                     | Ejemplo                       |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
| Variable      | Comienza por letra minúscula, y si tienen más de una palabra se colocan juntas y el resto comenzando por mayúsculas.           | `numAlumnos, suma`            |
| Constante     | En letras mayúsculas, separando las palabras con el guión bajo, por convenio el guión bajo no se utiliza en ningún otro sitio. | `TAM_MAX, PI`                 |
| Clase         | Comienza por letra mayúscula.                                                                                                  | `String, MiTipo`              |
| Método        | Comienza con letra minúscula y sigue las mismas reglas que las variables                                                       | `modificaValor, obtieneValor` |

#### 4.2.3 Palabras reservadas

Las palabras reservadas, a veces también llamadas palabras clave o keywords , son secuencias de caracteres formadas con letras ASCII cuyo uso se reserva al lenguaje y, por tanto, **no pueden utilizarse para crear identificadores.**

Las palabras reservadas en Java son:

|            |            |              |               |                |
| ---------- | ---------- | ------------ | ------------- | -------------- |
| `abstract` | `continue` | `for`        | `new`         | `switch`       |
| `assert`   | `default`  | `goto`       | `package`     | `synchronized` |
| `boolean`  | `do`       | `if`         | `private`     | `this`         |
| `break`    | `double`   | `implements` | `protected`   | `throw`        |
| `byte`     | `else`     | `import`     | `public`      | `throws`       |
| `case`     | `enum`     | `instanceof` | `return`      | `transient`    |
| `catch`    | `extends`  | `int`        | `short`       | `try`          |
| `char`     | `final`    | `interface`  | `static`      | `void`         |
| `class`    | `finally`  | `long`       | `strictfcode` | `volatile`     |
| `const`    | `float`    | `native`     | `super`       | `while`        |

Hay palabras reservadas que no se utilizan en la actualidad, como es el caso de `const` y `goto`, que apenas se utilizan en la actual implementación del lenguaje Java. Por otro lado, puede haber otro tipo de palabras o texto en el lenguaje que aunque no sean palabras reservadas tampoco se pueden utilizar para crear identificadores. Es el caso de `true` y `false` que, aunque puedan parecer palabras reservadas, porque no se pueden utilizar para ningún otro uso en un programa, técnicamente son **literales booleanos**. Igualmente, null es considerado un literal, no una palabra reservada.

> Cuando tras haber consultado la documentación de Java aún no tengas seguridad de cómo funciona alguna de sus características, pruébala en tu ordenador, y analiza cada mensaje de error que te dé el compilador para corregirlo. Busca en foros de Internet errores similares para ayudarte de la experiencia de otros usuarios y usuarias.

### 4.3 Salida por pantalla

La salida por pantalla en Java se hace con el objeto `System.out`. Este objeto es una instancia de la clase `PrintStream` del paquete `java.lang`. Si miramos la API de `PrintStream` obtendremos la variedad de métodos para mostrar datos por pantalla, algunos de estos son:

![clase PrintStream](.gitbook/assets/PROG01\_CONT\_R56\_PrintStream.png)

* `void print(String s):` Escribe una cadena de texto.
* `void println(String x):` Escribe una cadena de texto y termina la línea.

En la orden `print` y `println`, cuando queramos escribir un mensaje y el valor de una variable debemos utilizar el operador de concatenación de cadenas (+), por ejemplo:

```java
System.out.println(“Bienvenido, “ + nombre);
```

Escribe el mensaje de `"Bienvenido, Carlos"`, si el valor de la variable `nombre` es Carlos.

Existen unos caracteres especiales que se representan utilizando **secuencias de escape**:

| Secuencia de escape | Significado     | Secuencia de escape | Significado               |
| ------------------- | --------------- | ------------------- | ------------------------- |
| `\b`                | Retroceso       | `\r`                | Retorno de carro          |
| `\t`                | Tabulador       | `\''`               | Carácter comillas dobles  |
| `\n`                | Salto de línea  | `\'`                | Carácter comillas simples |
| `\f`                | Salto de página | `\\`                | Barra diagonal            |

### 4.4 Comentarios

Los comentarios son muy importantes a la hora de describir qué hace un determinado programa. A lo largo de la unidad los hemos utilizado para documentar los ejemplos y mejorar la comprensión del código. Para lograr ese objetivo, es normal que cada programa comience con unas líneas de comentario que indiquen, al menos, una breve descripción del programa, el autor del mismo y la última fecha en que se ha modificado.

Todos los lenguajes de programación disponen de alguna forma de introducir comentarios en el código. En el caso de Java, nos podemos encontrar los siguientes tipos de comentarios:

* **Comentarios de una sola línea**. Utilizaremos el delimitador `//` para introducir comentarios de sólo una línea.

```
// comentario de una sola línea
```

* **Comentarios de múltiples líneas**. Para introducir este tipo de comentarios, utilizaremos una barra inclinada y un asterisco (`/*`), al principio del párrafo y un asterisco seguido de una barra inclinada (`*/`) al final del mismo.

```
/* Esto es un comentario
de varias líneas */
```

* **Comentarios Javadoc**. Utilizaremos los delimitadores /\*\* y \*/. Al igual que con los comentarios tradicionales, el texto entre estos delimitadores será ignorado por el compilador. Este tipo de comentarios se emplean para generar documentación automática del programa. A través del programa javadoc, incluido en JavaSE , se recogen todos estos comentarios y se llevan a un documento en formato .html.

```
/** Comentario de documentación.
Javadoc extrae los comentarios del código y
genera un archivo html a partir de este tipo de comentarios
*/
```

{% hint style="warning" %}
Una buena práctica de programación es añadir en la última llave que delimita cada bloque de código, un comentario indicando a qué clase o método pertenece esa llave.
{% endhint %}

{% hint style="info" %}
Si quieres ir familiarizándote con la información que hay en la web de Oracle, en el siguiente enlace puedes encontrar más información sobre la herramienta Javadoc incluida en el Kit de Desarrollo de Java SE (en inglés): [Página oficial de Oracle sobre la herramienta Javadoc](http://download.oracle.com/javase/6/docs/technotes/guides/javadoc/index.html)
{% endhint %}

## 5. Trabajando con variables

Una vez descritos los elementos básicos de un programa en Java, en este apartado nos vamos a adentrar en su sintaxis, vamos a conocer los tipos de datos con los que trabaja, las operaciones que tienen definidas cada uno de ellos, utilizando ejemplos sencillos que nos muestren la utilidad de todo lo aprendido.

Para ello, vamos a tratar sobre cómo se almacenan y recuperan los datos de variables y cadenas en Java, y cómo se gestionan estos datos desde el punto de vista de la utilización de operadores. Trabajar con datos es fundamental en cualquier programa. Aunque ya hayas programado en este lenguaje, échale un vistazo al contenido del apartado, porque podrás repasar muchos conceptos.

{% hint style="info" %}
Ahora que vamos a empezar con la sintaxis de Java, quizás te interese tener a mano la documentación que ofrece la página web de Oracle sobre **Java SE**. La plataforma Java SE está formada principalmente por dos productos: el **JDK**, que contiene los **compiladores** y **depuradores** necesarios para programar, y el **JRE**, que proporciona las librerías o bibliotecas y la **JVM**, entre otra serie de componentes.

Puedes consultar información de la versión 8 de Java SE, en el siguiente enlace donde puedes encontrar toda la documentación sobre esta tecnología: [Documentación de Oracle sobre Java SE](https://docs.oracle.com/javase/8/)

Dentro de la documentación de Oracle sobre Java SE se encuentra el libro “The Java Language Specification”. Este libro está escrito por los inventores del lenguaje, y constituye una referencia técnica casi obligada sobre el mismo. Como mucha de la documentación oficial de Java, se encuentra en inglés: [The Java Language Specification](http://java.sun.com/docs/books/jls/index.html)
{% endhint %}

### 5.1 Las variables

Un programa maneja datos para hacer cálculos, presentarlos en informes por pantalla o impresora, solicitarlos al usuario, guardarlos en disco, etc. Para poder manejar esos datos, el programa los guarda en variables.\
Una **variable** es una zona en la memoria del computador con un valor que puede ser almacenado para ser usado más tarde en el programa. Las variables vienen determinadas por:

* Un nombre, que permite al programa acceder al valor que contiene en memoria. Debe ser un identificador válido.
* Un **tipo de dato**, que especifica qué clase de información guarda la variable en esa zona de memoria
* Un rango de valores que puede admitir dicha variable.

Al nombre que le damos a la variable se le llama **identificador**. Los identificadores permiten nombrar los elementos que se están manejando en un programa y como ya hemos visto, hay ciertos aspectos que debemos tener en cuenta al utilizarlos.

#### 5.1.1. Tipos de variables. Constantes I

En un programa nos podemos encontrar distintos tipos de variables. Las diferencias entre una variable y otra dependerán de varios factores, por ejemplo, el tipo de datos que representan, si su valor cambia o no a lo largo de todo el programa, o cuál es el papel que llevan a cabo en el programa. De esta forma, el lenguaje de programación Java define los siguientes tipos de variables:

1. **Variables de tipos primitivos y variables referencia,** según el tipo de información que contengan. En función de a qué grupo pertenezca la variable, tipos primitivos o tipos referenciados, podrá tomar unos valores u otros, y se podrán definir sobre ella unas operaciones u otras.
2. **Variables y constantes**, dependiendo de si su valor cambia o no durante la ejecución del programa. La definición de cada tipo sería:
   * Variables. Sirven para almacenar los datos durante la ejecución del programa, pueden estar formadas por cualquier tipo de dato primitivo o referencia. Su valor puede cambiar varias veces a lo largo de todo el programa.
   * Constantes o variables finales. Son aquellas variables cuyo valor no cambia a lo largo de todo el programa.
3. **Variables miembro y variables locales**, en función del lugar donde aparezcan en el programa. La definición concreta sería:
   * Variables miembro. Son las variables que se crean dentro de una **clase**, fuera de cualquier **método**. Pueden ser de tipos primitivos o referencias, variables o constantes.
   * Variables locales. Son las variables que se crean y usan dentro de un método o, en general, dentro de cualquier bloque de código. La variable deja de existir cuando la ejecución del bloque de código o el método finaliza. Al igual que las variables miembro, las variables locales también pueden ser de tipos primitivos o referencias.

#### Tipos de variables. Constantes II

El siguiente ejemplo muestra el código para la creación de varios tipos de variables. Como ya veremos en apartados posteriores, las variables necesitan declararse, a veces dando un valor y otras con un valor por defecto. Este programa crea una clase que contiene las siguientes variables:

* **Variable constante llamada** **`PI`**: esta variable por haberla declarado como constante no podrá cambiar su valor a lo largo de todo el programa.
* **Variable miembro llamada** **`x`:** Esta variable pertenece a la clase `ejemplovariables`. La variable x puede almacenar valores del tipo primitivo `int`. El valor de esta variable podrá ser modificado en el programa, normalmente por medio de algún otro método que se cree en la clase.
* **Variable local llamada** **`valorantiguo`:** Esta variable es local porque está creada dentro del método `obtenerX()`. Sólo se podrá acceder a ella dentro del método donde está creada, ya que fuera de él no existe.

![](.gitbook/assets/PROG01\_CONT\_R10\_ejemplovariables.jpg)

### 5.2 Los tipos de datos

En los **lenguajes fuertemente tipados**, a todo dato (constante, variable o expresión) le corresponde un tipo que es conocido antes de que se ejecute el programa.

El tipo limita el valor de la variable o expresión, las operaciones que se pueden hacer sobre esos valores, y el significado de esas operaciones. Esto es así porque **un tipo de dato no es más que una especificación de los valores que son válidos para esa variable , y de las operaciones que se pueden realizar con ellos.**

Debido a que el tipo de dato de una variable se conoce durante la revisión que hace el compilador para detectar errores, o sea en tiempo de compilación, esta labor es mucho más fácil, ya que no hay que esperar a que se ejecute el programa para saber qué valores va a contener esa variable. Esto se consigue con un control muy exhaustivo de los tipos de datos que se utilizan, lo cual tiene sus ventajas e inconvenientes, por ejemplo cuando se intenta asignar un valor de un tipo, a una variable de otro tipo. Sin embargo, en Java, puede haber conversión entre ciertos tipos de datos, como veremos posteriormente.

Ahora no es el momento de entrar en detalle sobre la conversión de tipos, pero sí debemos conocer con exactitud de qué tipos de datos dispone el lenguaje Java. Ya hemos visto que las variables, según la información que contienen, se pueden dividir en variables de tipos primitivos y variables referencia. Pero ¿qué es un tipo de dato primitivo? ¿Y un tipo referencia? Esto es lo que vamos a ver a continuación. Los tipos de datos en Java se dividen principalmente en dos categorías:

* **Tipos de datos sencillos o primitivos**. Representan valores simples que vienen predefinidos en el lenguaje; contienen valores únicos, como por ejemplo un carácter o un número.
* **Tipos de datos referencia.** Se definen con un nombre o referencia (puntero) que contiene la dirección en memoria de un valor o grupo de valores. Dentro de este tipo tenemos por ejemplo los vectores o arrays, que son una serie de elementos del mismo tipo, o las clases, que son los modelos o plantillas a partir de los cuales se crean los objetos.

#### **5.2.1 Tipos de datos primitivos**

Los tipos primitivos son aquéllos datos sencillos que constituyen los tipos de información más habituales: números, caracteres y valores lógicos o booleanos. Al contrario que en otros lenguajes de programación orientados a objetos, **en Java no son objetos**.

Una de las mayores ventajas de tratar con tipos primitivos en lugar de con objetos, es que el compilador de Java puede optimizar mejor su uso. Otra importante característica, es que cada uno de los tipos primitivos tiene **idéntico** tamaño y comportamiento en todas las versiones de Java y para cualquier tipo de ordenador. Esto quiere decir que no debemos preocuparnos de cómo se representarán los datos en distintas plataformas, y asegura la **portabilidad** de los programas, a diferencia de lo que ocurre con otros lenguajes. Por ejemplo, el tipo `int` siempre se representará con 32 bits, con signo, y en el formato de representación **complemento a 2**, en cualquier plataforma que soporte Java.

Hay una peculiaridad en los tipos de datos primitivos, y es que el tipo de dato char es considerado por el compilador como un tipo numérico, ya que los valores que guarda son el código Unicode correspondiente al carácter que representa, no el carácter en sí, por lo que puede operarse con caracteres como si se tratara de números enteros.

Por otra parte, a la hora de elegir el tipo de dato que vamos a utilizar ¿qué criterio seguiremos para elegir un tipo de dato u otro? Pues deberemos tener en cuenta cómo es la información que hay que guardar, si es de tipo texto, numérico, … y, además, qué rango de valores puede alcanzar. En este sentido, hay veces que aunque queramos representar un número sin decimales, tendremos que utilizar datos de tipo real.

Por ejemplo, el tipo de dato `int` no podría representar la población mundial del planeta, ya que el valor máximo que alcanza es de 2.147.483.647, siendo éste el número máximo de combinaciones posibles con 32 bits, teniendo en cuenta que la representación de los números enteros en Java utiliza complemento a 2. Si queremos representar el valor correspondiente a la población mundial del planeta, cerca de 7 mil millones de habitantes, tendríamos que utilizar al menos un tipo de dato `long`, o si tenemos problemas de espacio un tipo `float`. Sin embargo, los tipos reales tienen otro problema: la **precisión**. Vamos a ver más sobre ellos en el siguiente apartado.

| **Tipo** | **Descripción**                                                                      | **Bytes** | **Rango**                                                           | **Valor por default** |
| -------- | ------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------- | --------------------- |
| byte     | Entero muy corto                                                                     | 1         | -128 a 127                                                          | 0                     |
| short    | Entero corto                                                                         | 2         | -32,768 a 32,767                                                    | 0                     |
| int      | Entero                                                                               | 4         | -2,147,483,648 a 2,147,483,647                                      | 0                     |
| long     | Entero largo                                                                         | 8         | -9,223,372,036,854,775,808 a 9,223,372,036,854,775,807              | 0L                    |
| float    | Numero con punto flotante de precisión individual con hasta 7 dígitos significativos | 4         | +/-1.4E-45 (+/-1.4 times 10-45) a +/-3.4E38 (+/-3.4 times 1038)     | 0.0f                  |
| double   | Numero con punto flotante de precisión doble con hasta 16 dígitos significativos     | 8         | +/-4.9E-324 (+/-4.9 times 10-324) a +/-1.7E308 (+/-1.7 times 10308) | 0.0d                  |
| char     | Carácter [Unicode](http://en.wikipedia.org/wiki/Unicode)                             | 2         | \u0000 a \uFFFF                                                     | ‘\u0000’              |
| boolean  | Valor Verdadero o Falso                                                              | 1         | true o false                                                        | false                 |

**5.2.1.1 Tipos de datos reales**

El tipo de dato real permite representar cualquier número con decimales. Al igual que ocurre con los enteros, la mayoría de los lenguajes definen más de un tipo de dato real, en función del número de bits usado para representarlos. Cuanto mayor sea ese número:

* **Más grande podrá ser el número real representado en valor absoluto**
* **Mayor será la precisión** de la parte decimal

Entre cada dos números reales cualesquiera, siempre tendremos infinitos números reales, por lo que **la mayoría de ellos los representaremos de forma aproximada.** Por ejemplo, en la aritmética convencional, cuando dividimos 10 entre 3, el resultado es 3.3333333…, con la secuencia de 3 repitiéndose infinitamente. En el ordenador sólo podemos almacenar un número finito de bits, por lo que el almacenamiento de un número real será siempre una aproximación.

Los números reales se representan en coma flotante, que consiste en trasladar la coma decimal a la primera cifra significativa del valor, con objeto de poder representar el máximo de números posible.

Un número se expresa como: ![Valor igual a mantisa por dos elevado a exponente.](https://firebasestorage.googleapis.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MduJTOxgtvgHSkpgvN7%2Fuploads%2Fc4RPyjiK6IPDAvRyxIUL%2Ffile.png?alt=media)

En concreto, sólo se almacena la **mantisa** y el exponente al que va elevada la base. Los bits empleados por la mantisa representan la **precisión** del número real, es decir, el número de cifras decimales significativas que puede tener el número real, mientras que los bits del exponente expresan la diferencia entre el mayor y el menor número representable, lo que viene a ser el **intervalo de representación**.

En Java las variables de tipo `float` se emplean para representar los números en coma flotante de simple precisión de 32 bits, de los cuales 24 son para la mantisa y 8 para el exponente. La mantisa es un valor entre -1.0 y 1.0 y el exponente representa la potencia de 2 necesaria para obtener el valor que se quiere representar. Por su parte, las variables tipo `double` representan los números en coma flotante de doble precisión de 64 bits, de los cuales 53 son para la mantisa y 11 para el exponente.

{% hint style="success" %}
La mayoría de los programadores en Java emplean el tipo `double` cuando trabajan con datos de tipo real, es una forma de asegurarse de que los errores cometidos por las sucesivas aproximaciones sean menores. De hecho, Java considera los valores en coma flotante como de tipo `double` por defecto.
{% endhint %}

Con el objetivo de conseguir la máxima portabilidad de los programas, Java utiliza el estándar internacional **IEEE 754** para la representación interna de los números en coma flotante, que es una forma de asegurarse de que el resultado de los cálculos sea el mismo para diferentes plataformas.

{% hint style="info" %}
La siguiente página es la web oficial sobre el estándar internacional IEEE 754-2008 para representación de números en coma flotante (en inglés): [Notación IEEE 754](https://es.wikipedia.org/wiki/IEEE\_coma\_flotante)
{% endhint %}

**5.2.1.2 Literales de los tipos primitivos**

Un **literal**, **valor literal** o **constante literal** es un valor concreto para los tipos de datos primitivos del lenguaje, el tipo `String` o el tipo `null`.

Los **literales booleanos** tienen dos únicos valores que puede aceptar el tipo: `true` y `false`. Por ejemplo, con la instrucción `boolean encontrado = true;` estamos declarando una variable de tipo booleana a la cual le asignamos el valor literal `true`.

Los **literales enteros** se pueden representar en tres notaciones:

* **Decimal**: por ejemplo `20`. Es la forma más común.
* **Octal**: por ejemplo `024`. Un número en octal siempre empieza por cero, seguido de dígitos octales (del 0 al 7).
* **Hexadecimal**: por ejemplo `0x14`. Un número en hexadecimal siempre empieza por `0x` seguido de dígitos hexadecimales (del 0 al 9, de la ‘a’ a la ‘f’ o de la ‘A’ a la ‘F’).

Las constantes literales de tipo `long` se le debe añadir detrás una **l** ó **L**, por ejemplo `873L`, si no se considera por defecto de tipo `int`. Se suele utilizar **L** para evitar la confusión de la ele minúscula con 1.

Los **literales** **reales** o en coma flotante se expresan con coma decimal o en notación científica, o sea, seguidos de un exponente **e** ó **E**. El valor puede finalizarse con una f o una F para indica el formato float o con una d o una D para indicar el formato `double` (por defecto es `double`). Por ejemplo, podemos representar un mismo literal real de las siguientes formas: `13.2, 13.2D, 1.32e1, 0.132E2`. Otras constantes literales reales son por ejemplo: `.54, 31.21E-5, 2.f, 6.022137e+23f, 3.141e-9d.`

Un **literal carácter** puede escribirse como un carácter entre comillas simples como `'a', 'ñ', 'Z', 'p'`, etc. o por su código de la tabla Unicode, anteponiendo la secuencia de escape `‘\’` si el valor lo ponemos en octal o `‘\u’` si ponemos el valor en hexadecimal. Por ejemplo, si sabemos que tanto en ASCII como en Unicode, la letra A (mayúscula) es el símbolo número 65, y que 65 en octal es 101 y 41 en hexadecimal, podemos representar esta letra como `'\101'` en octal y `'\u0041'` en hexadecimal. Existen unos caracteres especiales que se representan utilizando secuencias de escape:

| Secuencia de escape | Significado     | Secuencia de escape | Significado               |
| ------------------- | --------------- | ------------------- | ------------------------- |
| `\b`                | Retroceso       | `\r`                | Retorno de carro          |
| `\t`                | Tabulador       | `\''`               | Carácter comillas dobles  |
| `\n`                | Salto de línea  | `\'`                | Carácter comillas simples |
| `\f`                | Salto de página | `\\`                | Barra diagonal            |

{% hint style="success" %}
**Normalmente, los objetos en Java deben ser creados con la orden `new`. Sin embargo, los literales String no lo necesitan ya que son objetos que se crean implícitamente por Java.**
{% endhint %}

Los **literales de cadenas de caracteres** se indican entre comillas dobles. En el ejemplo anterior “`El primer programa`” es un literal de tipo cadena de caracteres. Al construir una cadena de caracteres se puede incluir cualquier carácter Unicode excepto un carácter de retorno de carro, por ejemplo en la siguiente instrucción utilizamos la secuencia de escape \’’ para escribir dobles comillas dentro del mensaje:

```
String texto = "Juan dijo: \"Hoy hace un día fantástico…\"";
```

En el ejemplo anterior de tipos enumerados ya estábamos utilizando secuencias de escape, para introducir un salto de línea en una cadena de caracteres, utilizando el carácter especial `\n`.

#### 5.2.2 Declaración e inicialización

Llegados a este punto cabe preguntarnos ¿cómo se crean las variables en un programa? ¿Qué debo hacer antes de usar una variable en mi programa? Pues bien, como podrás imaginar, debemos crear las variables antes de poder utilizarlas en nuestros programas, indicando qué nombre va a tener y qué tipo de información va a almacenar, en definitiva, debemos **declarar la variable**.

Las variables se pueden declarar en cualquier bloque de código, dentro de llaves. Y lo hacemos indicando su identificador y el tipo de dato, separadas por comas si vamos a declarar varias a la vez, por ejemplo:

```
int numAlumnos = 15;
double radio = 3.14, importe = 102.95;
```

De esta forma, estamos declarando `numAlumnos` como una variable de tipo `int`, y otras dos variables `radio` e `importe` de tipo double. Aunque no es obligatorio, hemos aprovechado la declaración de las variables para inicializarlas a los valores 15, 3.14 y 102.95 respectivamente.

Si la variable va a permanecer inalterable a lo largo del programa, la declararemos como `constante`, utilizando la palabra reservada `final` de la siguiente forma:

```
final double PI = 3.1415926536;
```

En ocasiones puede que al declarar una variable no le demos valor, ¿qué crees que ocurre en estos casos? Pues que el compilador le asigna un valor por defecto, aunque depende del tipo de variable que se trate:

* Las **variables miembro** sí se inicializan automáticamente, si no les damos un valor. Cuando son de tipo numérico, se inicializan por defecto a `0`, si don de tipo carácter, se inicializan al carácter `null` (\0), si son de tipo `boolean` se les asigna el valor por defecto `false`, y si son tipo referenciado se inicializan a `null`.
* Las **variables locales** no se inicializan automáticamente. Debemos asignarles nosotros un valor antes de ser usadas, ya que si el compilador detecta que la variable se usa antes de que se le asigne un valor, produce un error. Por ejemplo en este caso:

```
int p;
int q = p; // error
```

dará error ya que se intenta usar la variable local p antes de haberse inicializado. El compilador detecta ese posible problema y produce un error del tipo **“La variable podría no haber sido inicializada”**.

#### 5.2.3 Tipos referenciados

A partir de los ocho tipos datos primitivos, se pueden construir otros tipos de datos. Estos tipos de datos se llaman **tipos referenciados** o **referencias**, porque se utilizan para almacenar la dirección de los datos en la memoria del ordenador.

```
int[] arrayDeEnteros;
Cuenta cuentaCliente;
```

En la primera instrucción declaramos una lista de números del mismo tipo, en este caso, enteros. En la segunda instrucción estamos declarando la variable u objeto `cuentaCliente` como una referencia de tipo `Cuenta`.

Como comentábamos al principio del apartado de Tipos de datos, cualquier aplicación de hoy en día necesita no perder de vista una cierta cantidad de datos. Cuando el conjunto de datos utilizado tiene características similares se suelen agrupar en estructuras para facilitar el acceso a los mismos, son los llamados **datos estructurados**. Son datos estructurados los **arrays, listas, árboles**, etc. Pueden estar en la memoria del programa en ejecución, guardados en el disco como ficheros, o almacenados en una base de datos.

Además de los ocho tipos de datos primitivos que ya hemos descrito, Java proporciona un tratamiento especial a los textos o cadenas de caracteres mediante el tipo de dato `String`. Java crea automáticamente un nuevo objeto de tipo `String` cuando se encuentra una cadena de caracteres encerrada entre comillas dobles. En realidad se trata de objetos, y por tanto son tipos referenciados, pero se pueden utilizar de forma sencilla como si fueran variables de tipos primitivos:

```
String mensaje;
mensaje = "El primer programa";
```

Hemos visto qué son las variables, cómo se declaran y los tipos de datos que pueden adoptar. Anteriormente hemos visto un ejemplo de creación de variables, en esta ocasión vamos a crear más variables, pero de distintos tipos primitivos y los vamos a mostrar por pantalla. Los tipos referenciados los veremos en la siguiente unidad.

Para mostrar por pantalla un mensaje utilizamos `System.out`, conocido como la salida estándar del programa. Este método lo que hace es escribir un conjunto de caracteres a través de la línea de comandos. Podemos utilizar `System.out.print` o `System.out.println`. En el segundo caso lo que hace el método es que justo después de escribir el mensaje, sitúa el cursor al principio de la línea siguiente. El texto en color gris que aparece entre caracteres `//` son comentarios que permiten documentar el código, pero no son tenidos en cuenta por el compilador y, por tanto, no afectan a la ejecución del programa.

![](.gitbook/assets/PROG01\_CONT\_R18\_Ejemplotipos.jpg)

#### 5.2.4 Tipos enumerados

Los **tipos de datos enumerados** son una forma de declarar una variable con un conjunto restringido de valores. Por ejemplo, los días de la semana, las estaciones del año, los meses, etc. Es como si definiéramos nuestro propio tipo de datos.

La forma de declararlos es con la palabra reservada `enum`, seguida del nombre de la variable y la lista de valores que puede tomar entre llaves. A los valores que se colocan dentro de las llaves se les considera como constantes, van separados por comas y deben ser valores únicos.

La lista de valores se coloca entre llaves, porque un tipo de datos `enum` no es otra cosa que una especie de clase en Java, y todas las clases llevan su contenido entre llaves.

Al considerar Java este tipo de datos como si de una clase se tratara, no sólo podemos definir los valores de un tipo enumerado, sino que también podemos definir operaciones a realizar con él y otro tipo de elementos, lo que hace que este tipo de dato sea más versátil y potente que en otros lenguajes de programación.

En el siguiente ejemplo puedes comprobar el uso que se hace de los tipos de datos enumerados. Tenemos una variable `Dias` que almacena los días de la semana. Para acceder a cada elemento del tipo enumerado se utiliza el nombre de la variable seguido de un punto y el valor en la lista. Más tarde veremos que podemos añadir métodos y campos o variables en la declaración del tipo enumerado, ya que como hemos comentado un tipo enumerado en Java tiene el mismo tratamiento que las clases.

![](.gitbook/assets/PROG01\_CONT\_R20\_EjemploEnumerados.jpg)

En este ejemplo hemos utilizado el método `System.out.print`. Como podrás comprobar si lo ejecutas, la instrucción número 18 escribe el texto que tiene entre comillas pero no salta a la siguiente línea, por lo que el la instrucción número 19 escribe justo a continuación.

Sin embargo, también podemos escribir varias líneas usando una única sentencia. Así lo hacemos en la instrucción número 20, la cual imprime como resultado tres líneas de texto. Para ello hemos utilizado un carácter especial, llamado **carácter escape** (`\`). Este carácter sirve para darle ciertas órdenes al compilador, en lugar de que salga impreso en pantalla. Después del carácter de escape viene otro carácter que indica la orden a realizar, juntos reciben el nombre de **secuencia de escape**. La secuencia de escape `\n` recibe el nombre de **carácter de nueva línea**. Cada vez que el compilador se encuentra en un texto ese carácter, el resultado es que mueve el cursor al principio de la línea siguiente. En el próximo apartado vamos a ver algunas de las secuencias de escape más utilizadas.

### 5.3 Operadores y expresiones

Los **operadores** llevan a cabo operaciones sobre un conjunto de datos u operandos, representados por literales y/o identificadores. Los operadores pueden ser unarios, binarios o terciarios, según el número de operandos que utilicen sean uno, dos o tres, respectivamente. Los operadores actúan sobre los tipos de datos primitivos y devuelven también un tipo de dato primitivo.

Los operadores se combinan con los literales y/o identificadores para formar expresiones. Una **expresión** es una combinación de operadores y operandos que se evalúa produciendo un único resultado de un tipo determinado.

El resultado de una expresión puede ser usado como parte de otra expresión o en una sentencia o instrucción. Las expresiones, combinadas con algunas palabras reservadas o por sí mismas, forman las llamadas **sentencias** o **instrucciones**.\
Por ejemplo, pensemos en la siguiente expresión Java:

```
i + 1
```

Con esta expresión estamos utilizando un operador aritmético para sumarle una cantidad a la variable i, pero es necesario indicar al programa qué hacer con el resultado de dicha expresión:

```
suma = i + 1;
```

Que lo almacene en una variable llamada `suma`, por ejemplo. En este caso ya tendríamos una acción completa, es decir, una sentencia o instrucción.

Más ejemplos de sentencias o instrucciones los tenemos en las declaraciones de variables, vistas en apartados anteriores, o en las estructuras básicas del lenguaje como sentencias condicionales o bucles, que veremos en unidades posteriores.

Como curiosidad comentar que las expresiones de asignación, al poder ser usadas como parte de otras asignaciones u operaciones, son consideradas tanto expresiones en sí mismas como sentencias.

#### 5.3.1 Operadores aritméticos

Los operadores aritméticos son aquellos operados que combinados con los operandos forman expresiones matemáticas o aritméticas.

Operadores aritméticos básicos:

| Operador | Operación Java                     | Expresión Java | Resultado |
| -------- | ---------------------------------- | -------------- | --------- |
|          |                                    |                |           |
| -        | Operador unario de cambio de signo | -10            | -10       |
| +        | Adición                            | 1.2 + 9.3      | 10.5      |
| -        | Sustracción                        | 312.5 – 12.3   | 300.2     |
| \*       | Multiplicación                     | 1.7 \* 1.2     | 1.02      |
| /        | División (entera o real)           | 0.5 / 0.2      | 2.5       |
| **%**    | Resto de la división entera        | 25 % 3         | 1         |

El resultado de este tipo de expresiones depende de los operandos que utilicen:

| Tipo de los operandos                                          | Resultado |
| -------------------------------------------------------------- | --------- |
| Un operando de tipo `long` y ninguno real (`float` o `double`) | `long`    |
| Ningún operando de tipo `long` ni real (`float` o `double`)    | `int`     |
| Al menos un operando de tipo `double`                          | `double`  |
| Al menos un operando de tipo `float` y ninguno `double`        | `float`   |

Otro tipo de operadores aritméticos son los operadores unarios incrementales y decrementales. Producen un resultado del mismo tipo que el operando, y podemos utilizarlos con **notación prefija**, si el operador aparece antes que el operando, o **notación** **postfija**, si el operador aparece después del operando. En la tabla puedes un ejemplo de de utilización de cada operador incremental.

Operadores incrementales en Java:

| Tipo operador    | Expresión Java                                                   |                                                                   |
| ---------------- | ---------------------------------------------------------------- | ----------------------------------------------------------------- |
| ++ (incremental) | <p>Prefija: </p><p>x=3;</p><p>y=++x;  // x vale 4 e y vale 4</p> | <p>Postfija:</p><p>x=3; </p><p>y=x++;  // x vale 4 e y vale 3</p> |
| -- (decremental) | 5-- // el resultado es 4                                         |                                                                   |

![](.gitbook/assets/PROG01\_CONT\_R25\_Operadoresaritmeticos.jpg)

En el ejemplo vemos un programa básico que utiliza operadores aritméticos. Observa que usamos `System.out.printf` para mostrar por pantalla un texto formateado. El texto entre dobles comillas son los argumentos del método `printf` y si usamos más de uno, se separan con comas. Primero indicamos cómo queremos que salga el texto, y después el texto que queremos mostrar. Fíjate que con el primer `%s` nos estamos refiriendo a una variable de tipo `String`, o sea, a la primera cadena de texto, con el siguiente `%s` a la segunda cadena y con el último `%s` a la tercena. Con `%f` nos referimos a un argumento de tipo float, etc.

#### 5.3.2 Operadores de asignación

El principal operador de esta categoría es el operador asignación `“=”,` que permite al programa darle un valor a una variable, y ya hemos utilizado varias ocasiones en esta unidad. Además de este operador, Java proporciona otros operadores de asignación combinados con los operadores aritméticos, que permiten abreviar o reducir ciertas expresiones.

Por ejemplo, el operador `“+=”` suma el valor de la expresión a la derecha del operador con el valor de la variable que hay a la izquierda del operador, y almacena el resultado en dicha variable. En la siguiente tabla se muestran todos los operadores de asignación compuestos que podemos utilizar en Java.

Operaciones de asignación combinados en Java:

| Operador | Ejemplo en Java | Expresión equivalente |
| -------- | --------------- | --------------------- |
| `+=`     | `op1 += op2`    | `op1 = op1 + op2`     |
| `-=`     | `op1 -= op2`    | `op1 = op1 - op2`     |
| `*=`     | `op1 *= op2`    | `op1 = op1 * op2`     |
| `/=`     | `op1 /= op2`    | `op1 = op1 / op2`     |
| `%=`     | `op1 %= op2`    | `op1 = op1 % op2`     |

Un ejemplo de operadores de asignación combinados lo tenemos a continuación:

![](.gitbook/assets/PROG01\_CONT\_R27\_Ejemplocombinados.jpg)

#### 5.3.3 Operaciones de relación

Los operadores relacionales se utilizan para comparar datos de tipo primitivo (numérico, carácter y booleano). El resultado se utilizará en otras expresiones o sentencias, que ejecutarán una acción u otra en función de si se cumple o no la relación.

Estas expresiones en Java dan siempre como resultado un valor booleano true o false. En la tabla siguiente aparecen los operadores relacionales en Java.

Operaciones relacionales en Java:

| Operador | Ejemplo en Java | Significado               |
| -------- | --------------- | ------------------------- |
| `==`     | `op1 == op2`    | op1 igual a op2           |
| `!=`     | `op1 != op2`    | op1 distinto de op2       |
| `>`      | `op1 > op2`     | op1 mayor que op2         |
| `<`      | `op1 < op2`     | op1 menor que op2         |
| `>=`     | `op1 >= op2`    | op1 mayor o igual que op2 |
| `<=`     | `op1 <= op2`    | op1 menor o igual que op2 |

Hasta ahora hemos visto ejemplos que creaban variables y se inicializaban con algún valor. Pero ¿y si lo que queremos es que el usuario introduzca un valor al programa? Entonces debemos agregarle interactividad a nuestro programa, por ejemplo utilizando la clase `Scanner`. Aunque no hemos visto todavía qué son las clases y los objetos, de momento vamos a pensar que la clase `Scanner` nos va a permitir leer los datos que se escriben por teclado, y que para usarla es necesario importar el paquete de clases que la contiene. El código del ejemplo lo tienes a continuación. El programa se quedará esperando a que el usuario escriba algo en el teclado y pulse la tecla intro. En ese momento se convierte lo leído a un valor del tipo `int` y lo guarda en la variable indicada. Además de los operadores relacionales, en este ejemplo utilizamos también el operador condicional, que compara si los números son iguales. Si lo son, devuelve la cadena iguales y sino, la cadena distintos.

![](.gitbook/assets/PROG01\_CONT\_R30\_Ejemplorelacionalycondicional.jpg)

#### 5.3.4 Precedencia de operadores

El orden de precedencia de los operadores determina la secuencia en que deben realizarse las operaciones cuando en una expresión intervienen operadores de distinto tipo.

Las reglas de precedencia de operadores que utiliza Java coinciden con las reglas de las expresiones del álgebra convencional. Por ejemplo:

* La multiplicación, división y resto de una operación se evalúan primero. Si dentro de la misma expresión tengo varias operaciones de este tipo, empezaré evaluándolas de izquierda a derecha.
* La suma y la resta se aplican después que las anteriores. De la misma forma, si dentro de la misma expresión tengo varias sumas y restas empezaré evaluándolas de izquierda a derecha.

A la hora de evaluar una expresión es necesario tener en cuenta la **asociatividad** de los operadores. La asociatividad indica qué operador se evalúa antes, en condiciones de igualdad de precedencia. Los operadores de asignación, el operador condicional (`?:`), los operadores incrementales (`++, --`) y el casting son asociativos por la derecha. El resto de operadores son asociativos por la izquierda, es decir, que se empiezan a calcular en el mismo orden en el que están escritos: de izquierda a derecha. Por ejemplo, en la expresión siguiente:

```
10 / 2 * 5
```

Realmente la operación que se realiza es `(10 / 2 ) * 5`, porque ambos operadores, división y multiplicación, tienen igual precedencia y por tanto se evalúa primero el que antes nos encontramos por la izquierda, que es la división. El resultado de la expresión es `25`. Si fueran asociativos por la derecha, puedes comprobar que el resultado sería diferente, primero multiplicaríamos `2 * 5` y luego dividiríamos entre `10`, por lo que el resultado sería 1. En esta otra expresión:

```
x = y = z = 1
```

Realmente la operación que se realiza es `x = (y = (z = 1))`. Primero asignamos el valor de `1` a la variable `z`, luego a la variable `y`, para terminar asignando el resultado de esta última asignación a `x`. Si el operador asignación fuera asociativo por la izquierda esta operación no se podría realizar, ya que intentaríamos asignar a `x` el valor de `y`, pero `y` aún no habría sido inicializada.

En la tabla se detalla el orden de precedencia y la asociatividad de los operadores que hemos comentado en este apartado. Los operadores se muestran de mayor a menor precedencia.

Orden de precedencia de operadores en Java

| Operador                                                  | Tipo                      | Asociatividad |
| --------------------------------------------------------- | ------------------------- | ------------- |
| `++ --`                                                   | Unario, notación postfija | Derecha       |
| <p><code>++ -- + -</code><br> <code>(cast) ! ~</code></p> | Unario, notación prefija  | Derecha       |
| `* / %`                                                   | Aritméticos               | Izquierda     |
| `+ -`                                                     | Aritméticos               | Izquierda     |
| `<< >> >>>`                                               | Bits                      | Izquierda     |
| `< <= > >=`                                               | Relacionales              | Izquierda     |
| `== !=`                                                   | Relacionales              | Izquierda     |
| `&`                                                       | Lógico, Bits              | Izquierda     |
| `^`                                                       | Lógico, Bits              | Izquierda     |
| `\|`                                                      | Lógico, Bits              | Izquierda     |
| `&&`                                                      | Lógico                    | Izquierda     |
| `\|\|`                                                    | Lógico                    | Izquierda     |
| `?:`                                                      | Operador condicional      | Derecha       |
| <p><code>= += -= *=</code><br> <code>/= %=</code></p>     | Asignación                | Derecha       |

### 5.4 Conversión de tipo

Imagina que queremos dividir un número entre otro ¿tendrá decimales el resultado de esa división? Podemos pensar que siempre que el denominador no sea divisible entre el divisor, tendremos un resultado con decimales, pero no es así. Si el denominador y el divisor son variables de tipo entero, el resultado será entero y no tendrá decimales. Para que el resultado tenga decimales necesitaremos hacer una **conversión de tipo**.

Las conversiones de tipo se realizan para hacer que el resultado de una expresión sea del tipo que nosotros deseamos, en el ejemplo anterior para hacer que el resultado de la división sea de tipo real y, por ende, tenga decimales. Existen dos tipos de conversiones:

* **Conversiones automáticas**. Cuando a una variable de un tipo se le asigna un valor de otro tipo numérico con menos bits para su representación, se realiza una conversión automática. En ese caso, el valor se dice que es promocionado al tipo más grande (el de la variable), para poder hacer la asignación. También se realizan conversiones automáticas en las operaciones aritméticas, cuando estamos utilizando valores de distinto tipo, el valor más pequeño se promociona al valor más grande, ya que el tipo mayor siempre podrá representar cualquier valor del tipo menor (por ejemplo, de `int` a `long` o de `float` a `double`).
* **Conversiones explícitas**. Cuando hacemos una conversión de un tipo con más bits a un tipo con menos bits. En estos casos debemos indicar que queremos hacer la conversión de manera expresa, ya que se puede producir una pérdida de datos y hemos de ser conscientes de ello. Este tipo de conversiones se realiza con el **operador `cast`**. El operador `cast` es un operador unario que se forma colocando delante del valor a convertir el tipo de dato entre paréntesis. Tiene la misma precedencia que el resto de operadores unarios y se asocia de izquierda a derecha.

Debemos tener en cuenta que **un valor numérico nunca puede ser asignado a una variable de un tipo menor en rango, si no es con una conversión explícita**. Por ejemplo:

```
int a;
byte b;
a = 12;               // no se realiza conversión alguna  
b = 12;               // se permite porque 12 está dentro
                      // del rango permitido de valores para b
b = a;                // error, no permitido (incluso aunque
                      // 12 podría almacenarse en un byte)
byte b = (byte) a;    // Correcto, forzamos conversión explícita
```

En el ejemplo anterior vemos un caso típico de error de tipos, ya que estamos intentando asignarle a `b` el valor de `a`, siendo `b` de un tipo más pequeño. Lo correcto es promocionar `a` al tipo de datos `byte`, y entonces asignarle su valor a la variable `b`.

{% hint style="info" %}
En el siguiente enlace viene información importante sobre cómo se producen las conversiones de tipos en Java, tanto automáticas como explícitas: [Conversión de Tipos de Datos en Java](anexo-i.-conversion-de-tipos-de-datos-en-java.md)
{% endhint %}

## 6. Estructuras de repetición

Nuestros programas ya son capaces de operar con datos de tipo entero y real, pero aún hemos de aprender un conjunto de estructuras que nos permita repetir una secuencia de instrucciones determinada. La función de estas estructuras es repetir la ejecución de una serie de instrucciones teniendo en cuenta una condición.

A este tipo de estructuras se las denomina **estructuras de repetición**, estructuras repetitivas, **bucles** o estructuras **iterativas**. En Java existen cuatro clases de bucles:

* Bucle `for` (repite para)
* Bucle `for/in` (repite para cada)
* Bucle `While` (repite mientras)
* Bucle `Do While` (repite hasta)

Los bucles `for` y `for/in` se consideran bucles **controlados por contador**. Por el contrario, los bucles `while` y `do...while` se consideran bucles **controlados por sucesos.**

La utilización de unos bucles u otros para solucionar un problema dependerá en gran medida de las siguientes preguntas:

* ¿Sabemos **a priori** cuántas veces necesitamos repetir un conjunto de instrucciones?
* ¿Sabemos si hemos de repetir un conjunto de instrucciones si una condición satisface un conjunto de valores?
* ¿Sabemos hasta cuándo debemos estar repitiendo un conjunto de instrucciones?
* ¿Sabemos si hemos de estar repitiendo un conjunto de instrucciones mientras se cumpla una condición?

En esta UD nos vamos a centrar en los bucles `for`, dejando el resto para UDs posteriores.

### 6.1 Estructuras FOR

Hemos indicado anteriormente que el bucle `for` es un bucle controlado por contador. Este tipo de bucle tiene las siguientes características:

* Se ejecuta un número determinado de veces.
* Utiliza una variable contadora que controla las iteraciones del bucle.

En general, existen tres operaciones que se llevan a cabo en este tipo de bucles:

* Se inicializa la variable contadora.
* Se evalúa el valor de la variable contador, por medio de una comparación de su valor con el número de iteraciones especificado.
* Se modifica o actualiza el valor del contador a través de incrementos o decrementos de éste, en cada una de las iteraciones.

![](.gitbook/assets/PROG01\_CONT\_R05\_diagramafor.jpg)

{% hint style="danger" %}
La inicialización de la variable contadora debe realizase correctamente para garantizar que el bucle se lleve a cabo, al menos, la primera repetición de su código interno.

La condición de terminación del bucle debe variar en el interior del mismo, de no ser así, podemos caer en la creación de un bucle infinito. Cuestión que se debe evitar por todos los medios.

Es necesario estudiar el número de veces que se repite el bucle, pues debe ajustarse al número de veces estipulado.
{% endhint %}

**Sintaxis:**

```java
for (inicialización; condición; iteración)
{
    sentencia1;
    sentencia2;
    ...
    sentenciaN;
}
```

* _Inicialización_ es una expresión en la que se inicializa una variable de control, que será la encargada de controlar el final del bucle.
* _Condición_ es una expresión que evaluará la variable de control. Mientras la condición se cumpla, el cuerpo del bucle estará repitiéndose. Cuando la condición sea falsa, terminará la ejecución del bucle.
* _Iteración_ indica la manera en la que la variable de control va cambiando en cada iteración del bucle. Podrá ser mediante incremento o decremento, y no solo de uno en uno.

```java
public class repetitiva_for {
     /* En este ejemplo se utiliza la estructura repetitiva for
     * para representar en pantalla la tabla de multiplicar del siete 
     */
    public static void main(String[] args) {
        // Declaración e inicialización de variables
        int numero = 7;
        int contador;
        int resultado=0;
        
        //Salida de información
        System.out.println ("Tabla de multiplicar del " + numero);
        System.out.println (".............................. ");
        
        //Utilizamos ahora el bucle for
        for (contador=1; contador<=10; contador++)
        /* La cabecera del bucle incorpora la inicialización de la variable
         * de control, la condición de multiplicación hasta el 10 y el
         * incremento de dicha variable de uno en uno en cada iteración del
         * bucle. 
         * En este caso contador++ incrementará en una unidad el valor de 
         * dicha variable.
         */
            
        {
            resultado = contador * numero; 
            System.out.println(numero + " x " + contador + " = " + resultado);
            /* A través del operador + aplicado a cadenas de caracteres, 
             * concatenamos los valores de las variables con las cadenas de
             * caracteres que necesitamos para representar correctamente la
             * salida de cada multiplicación.
             */
        }
    }    
}
```

## 7. Descomposición de programas

Cuando nos enfrentarnos a un problema, conviene dividirlo en partes más manejables y sencillas de crear y mantener. De este modo además, conseguiremos programas más estructurados y comprensibles, y evitaremos la redundancia de código en nuestras aplicaciones.

Para ello, Java proporciona los métodos. Estos permiten agrupar un conjunto de instrucciones que realizan una determinada tarea e identificarlas mediante un nombre. De esta manera, podemos crear un método y luego utilizarlo todas las veces que queramos mediante su identificador.

Para poder trabajar con métodos, primero tendremos que **declarar** el método:

```
public static void identificadoMetodo() {
    sentencia 1;
    sentencia 2;
    ...
    sentencia N;
}
```

Y luego realizar **llamadas** a él donde los queramos utilizar:

```
identificadorMetodo();
```

{% hint style="warning" %}
Por ahora, hasta saber más sobre los métodos, los vamos a declarar **todos como** **public static void** y los vamos a utilizar para descomponer y estructurar programas.

Más adelante, iremos viendo otras características de los métodos.
{% endhint %}
