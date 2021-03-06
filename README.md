# BIBLIOJAVA

### Aplicación en Java para gestionar una biblioteca a través de consola.

Esta aplicación ha sido desarrollada como parte del trabajo práctico del módulo de Programación del Ciclo Formativo de Grado Superior en Desarrollo de Aplicaciones Web, en el Instituto de Educación Secundaria Polígono Sur de Sevilla.

Su función y objetivo es el aprendizaje y manejo de las distintas herramientas que proporciona Java, por lo que se irá actualizando a lo largo de los meses.

Actualmente la aplicación funciona con vectores (_arrays dinámicos_), por lo que **la información almacenada durante la ejecución se perderá** una vez se cierre el programa. Más adelante la aplicación incorporará persistencia de datos, primero mediante ficheros y luego en base de datos.

1. [Antes de empezar](#1)
2. [Creación de paquetes](#2)
3. [Ejecución](#3)
4. [Funcionamiento](#4)
5. [Funciones en desarrollo](#5)
6. [Lista de cambios](#6)

### <a name="1"></a>Antes de empezar

Para una correcta y más fácil ejecución de la aplicación se recomienda el uso de un entorno de desarrollo integrado o IDE, caso de **_Eclipse_**, que es en el que se ha desarrollado el código.

### <a name="2"></a>Creación de paquetes

En el IDE, es necesario crear un proyecto (podemos llamarlo _Biblioteca_) y dentro de éste un paquete, que puede denominarse igual. Dentro se ubicarán todas las clases que se incluyen en este proyecto.

### <a name="3"></a>Ejecución

Para que la aplicación funcione debemos ejecutar la clase **Biblioteca.java**, que es la clase ejecutable donde se encuentra el método _main_ que llama a las demás clases de objetos.

### <a name="4"></a>Funcionamiento

Al ejecutar la aplicación aparecerá en la consola un menú que ofrecerá al usuario varias opciones:

1. Gestión de libros.
2. Gestión de revistas.
3. Gestión de CD-ROM.
4. Gestión de usuarios.
5. Realizar préstamo.
6. Devolver préstamo.
7. Mostrar préstamos.
0. Salir.

Las cuatro primeras opciones dan acceso a sendos nuevos menús que permiten la gestión de los distintos materiales y de los usuarios de la biblioteca, y que cuentan con las siguientes opciones:

1. Añadir recurso / usuario.
2. Eliminar recurso / usuario.
3. Modificar recurso / usuario.
4. Mostrar recursos / usuarios.
0. Volver al menú principal.

Además, la gestión de revistas incluye una quinta opción: gestión de artículos. A través de ella podemos acceder a otro menú para gestionar los artículos que contiene cada revista, y que cuenta con las siguientes opciones:

1. Añadir artículo.
2. Eliminar artículo.
3. Modificar artículo.
4. Mostrar artículos.
0. Volver al menú principal.

Las opciones 5, 6 y 7 del menú principal de la biblioteca permiten la gestión de los préstamos de material de distinto tipo que los usuarios de la biblioteca solicitan o devuelven. La opción 7 ("Mostrar préstamos"), permite comprobar el historial de préstamos y devoluciones de material.

El usuario podrá interactuar con la aplicación a través del teclado tanto para elegir la opción deseada como para introducir los distintos datos que se le irán solicitando.

La aplicación finalizará cuando en el menú principal se pulse 0. **Al finalizar la aplicación se perderá toda la información introducida**.

### <a name="5"></a>Funciones en desarrollo

Algunas funciones que se encuentran en desarrollo y que se ofrecerán en las siguientes versiones son:

* Persistencia de datos (sobre ficheros).
* Gestión de las fechas de los préstamos con la clase Calendar. Automatización de las fechas de devolución al realizar un préstamo.
* Inclusión de menús de selección en las funciones que lo requieran (por ejemplo, en la selección de material durante los préstamos).
* Corrección de errores y perfeccionamiento de funciones.

### <a name="6"></a>Lista de cambios

A continuación se detallan las distintas versiones de esta aplicación y los principales cambios o funciones añadidas:

**[9/01/2018] Bibliojava 0.1.0:**

* Almacenamiento con arrays estáticos (persistencia en memoria).
* Gestión de artículos (como material independiente), libros, revistas, CD-ROM y usuarios.

**[19/01/2018] Bibliojava 0.2.0:**

* Sustitución de los _arrays_ estáticos por _arrays_ dinámicos (vectores). Reescritura de funciones.
* Gestión de préstamos: posibilidad de realizar y devolver préstamos de distintos materiales.
* Cambios en la gestión de artículos: las revistas pasan a estar conformadas por artículos, de modo que los artículos dejan de ser un material independiente. El acceso a la gestión de artículos desaparece del menú principal y se realiza a través del menú de gestión de revistas. Cada revista tendrá su propia lista de artículos.
* Corrección de errores.
