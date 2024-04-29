# Prestamos-MVC
**Flores Alvarado Julio Cesar
**Castillo Guadarrama Brenda
Ensayo de un Modelo-Vista-Controlador
Instituto Tecnol�gico de Tl�huac
Ingenier�a en Sistemas Computacionales
Grupo: 8S2. Programaci�n Web PHP con MVC
21 de marzo de 2024**

#### ------------------------------------------------------------------

#�ndice

#####***Resumen		1***

#####***Introducci�n	1***

#####***Desarrollo	1***

#####***Conclusiones	12***

#####***Referencias	13***

#### ------------------------------------------------------------------

# ***Resumen***

*El Modelo-Vista-Controlador (MVC) es un patr�n arquitect�nico ampliamente utilizado en el desarrollo de software. Este enfoque divide una aplicaci�n en tres componentes principales: el modelo, que representa los datos y la l�gica de negocio; la vista, que se encarga de la presentaci�n de la informaci�n al usuario; y el controlador, que act�a como intermediario entre el modelo y la vista. Este ensayo explora la importancia del MVC en el desarrollo de software moderno, sus beneficios y su aplicaci�n en diferentes contextos.*

#### ------------------------------------------------------------------

#***Introducci�n***
*En el panorama actual del desarrollo de software, el modularidad, la escalabilidad y la mantenibilidad son aspectos cruciales para el �xito de un proyecto. El patr�n MVC surge como una soluci�n elegante para abordar estos desaf�os al promover la separaci�n de preocupaciones y la organizaci�n estructurada del c�digo. Al dividir una aplicaci�n en tres componentes distintos pero interconectados, MVC permite un desarrollo m�s ordenado, facilita la reutilizaci�n de c�digo y promueve una mayor flexibilidad y adaptabilidad a medida que los requerimientos evolucionan.*

#### ------------------------------------------------------------------

# ***Desarrollo***
Estos archivos son utilizados para crear una p�gina web con funcionalidades b�sicas como la estructura de la cuadr�cula, botones, formularios, barras de desplazamiento, alertas, ventanas emergentes y m�s. Tambi�n se utilizan para aplicar estilos a la p�gina web y mejorar la experiencia del usuario.

![]("C:\Users\Julio Alvarado\Documents\Julio\Materias\Noveno Semestre\Prog. PHP con MVC\Proyecto\Ensayo M-V-C\Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.001.jpeg")

El Modelo-Vista-Controlador se compone de tres elementos clave:

####***Modelo:***

*El modelo representa los datos subyacentes de la aplicaci�n y la l�gica de negocio asociada. Es responsable de manejar la manipulaci�n y el almacenamiento de los datos, as� como de aplicar las reglas de negocio necesarias para procesarlos correctamente. Al separar la l�gica de negocio del resto de la aplicaci�n, el modelo facilita la reutilizaci�n y la prueba de la funcionalidad de manera independiente.*

####**LoginModelo.php**

Define una clase loginModelo que extiende otra clase llamada mainModel, indicando que probablemente herede funcionalidades relacionadas con la interacci�n con la base de datos. Dentro de esta clase, hay un m�todo protegido llamado iniciar\_sesion\_modelo($datos), que se encarga de iniciar sesi�n en el sistema. Este m�todo ejecuta una consulta SQL preparada para seleccionar los datos de usuario correspondientes a las credenciales proporcionadas. El resultado de la consulta se devuelve para su posterior procesamiento, como verificar si las credenciales son v�lidas.

####**mainModel.php**

Esta clase proporciona una serie de funciones esenciales para realizar operaciones comunes en un sistema, como interactuar con la base de datos, validar datos, encriptar y desencriptar informaci�n, y gestionar la paginaci�n de resultados. Esto promueve la reutilizaci�n de c�digo y la implementaci�n eficiente de funcionalidades en el sistema.

####**usuarioModelo.php**

Estos m�todos ofrecen una interfaz para realizar operaciones comunes de CRUD (Crear, Leer, Actualizar, Eliminar) en la tabla de usuarios, promoviendo la modularidad y reutilizaci�n del c�digo.

####**vistasModelo.php**

Este c�digo determina la vista que se debe cargar en funci�n de la solicitud del usuario, asegurando que solo se acceda a vistas permitidas y manejando adecuadamente los casos donde la vista solicitada no existe.

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.002.jpeg)

####***Vista:***

*La vista es la interfaz de usuario que presenta la informaci�n al usuario final de manera comprensible y atractiva. Su principal funci�n es mostrar los datos proporcionados por el modelo y permitir la interacci�n del usuario con la aplicaci�n. Al separar la l�gica de presentaci�n del resto del sistema, la vista facilita la adaptaci�n a diferentes dispositivos y plataformas sin afectar la l�gica subyacente.*

####**Index.php**

*Este c�digo PHP carga la configuraci�n de la aplicaci�n y el controlador de vistas, crea una instancia del controlador de vistas y llama a un m�todo en ese controlador para obtener y renderizar la plantilla principal de la aplicaci�n.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.003.png)

####**.htacces**

*Reescribe cualquier solicitud de URL que consista en letras, n�meros, barras inclinadas, o los caracteres �, �, o -, a index.php, pasando el valor capturado como un par�metro views. Por ejemplo, una solicitud a mi\_pagina se reescribir�a internamente como index.php?views=mi\_pagina.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.004.png)

####**Plantilla.php**

*Este c�digo HTML con incrustaciones de PHP establece la estructura b�sica de una p�gina web din�mica. Incluye un encabezado con metadatos y un t�tulo obtenido de una constante PHP. Se carga un archivo PHP para enlaces externos. El cuerpo del documento contiene l�gica condicional en PHP para gestionar qu� contenido mostrar, dependiendo de la solicitud. Se verifica la existencia de variables de sesi�n y se redirecciona al inicio de sesi�n si es necesario. La p�gina principal incluye una barra lateral de navegaci�n y el contenido principal se carga din�micamente seg�n la vista solicitada. Finalmente, se incluyen archivos PHP adicionales para manejar el cierre de sesi�n y se cargan scripts necesarios para la funcionalidad de la p�gina.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.005.png)

####**NavBar.php**

*Este c�digo HTML representa una barra de navegaci�n con tres enlaces. El primer enlace activa/desactiva una barra lateral de navegaci�n. El segundo enlace lleva a una p�gina de actualizaci�n de usuario, con la URL construida din�micamente usando PHP para incluir el ID de sesi�n cifrado. El tercer enlace parece ser un bot�n de cierre de sesi�n.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.006.png)

####**NavLateral.php**

*Este bloque de c�digo HTML con incrustaciones de PHP describe la estructura de una barra de navegaci�n lateral utilizada en una aplicaci�n web. Est� compuesto por dos elementos principales dentro de un contenedor <section>. Primero, un fondo oscuro transparente que se muestra cuando la barra lateral est� activa, y luego el contenido real de la barra lateral, que incluye un avatar de usuario, una barra de separaci�n y un men� de navegaci�n. Este men� de navegaci�n contiene una lista de elementos de men� representados por enlaces, generados din�micamente utilizando PHP para construir las URL. Algunos elementos de men� pueden estar condicionados seg�n el nivel de privilegio del usuario, mostrando ciertas opciones de men� solo para usuarios con privilegios espec�ficos.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.007.png)

####**Script.php**

*Describe la inclusi�n de varios archivos JavaScript en una p�gina web. Los archivos incluidos son principalmente bibliotecas y scripts personalizados esenciales para la funcionalidad y el dise�o de la p�gina. Esto incluye bibliotecas como jQuery, Popper, Bootstrap, y Bootstrap Material Design, que proporcionan funcionalidades como manipulaci�n del DOM, posicionamiento de elementos emergentes, estilos y componentes de interfaz de usuario. Adem�s, se incluyen scripts personalizados como **main.js** y **alertas.js**, que pueden proporcionar funcionalidades espec�ficas y personalizadas para la p�gina web.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.008.png)

####**LogOut.php**

*Este script implementa la funcionalidad de salida del sistema al hacer clic en un bot�n espec�fico. Utiliza SweetAlert para mostrar un cuadro de di�logo de confirmaci�n. Si el usuario confirma la salida, se env�a una solicitud AJAX al servidor para cerrar la sesi�n del usuario actual. La solicitud incluye el token de sesi�n y el nombre de usuario cifrados para garantizar la seguridad de la operaci�n. Una vez completada la solicitud, se procesa la respuesta del servidor, probablemente mostrando alertas o notificaciones al usuario. En resumen, este sistema proporciona una forma segura y controlada para que los usuarios salgan del sistema.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.009.png)

####**Link.php**

*Describe la inclusi�n de varios archivos CSS y JavaScript en una p�gina web. Los archivos incluidos proporcionan estilos y funcionalidades para la interfaz de usuario de la p�gina. Esto incluye estilos de normalizaci�n (**normalize.css**), estilos y componentes de Bootstrap (**bootstrap.min.css**), estilos de dise�o de material de Bootstrap (**bootstrap-material-design.min.css**), iconos de Font Awesome (**all.css**), estilos para alertas personalizadas (**sweetalert2.min.css**), y estilos para barras de desplazamiento personalizadas (**jquery.mCustomScrollbar.css**). Adem�s, se incluye un archivo JavaScript para las alertas personalizadas (**sweetalert2.min.js**). Estos archivos ayudan a establecer la apariencia y el comportamiento deseado de la p�gina web.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.010.png)

*El sistema de pr�stamos cuenta con una serie de archivos de vista en el directorio "vistas". Cada archivo .php en este directorio representa una vista espec�fica dentro del sistema, desde la visualizaci�n de clientes y �tems hasta la gesti�n de reservas y usuarios. Estas vistas proporcionan una interfaz para realizar diversas acciones, como agregar nuevos clientes o buscar �tems disponibles.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.011.jpeg)

*Los archivos en la carpeta assets son esenciales para el funcionamiento del sistema de pr�stamos. Estos archivos proporcionan las im�genes, iconos, JavaScript, CSS y fuentes que se utilizan para crear una interfaz de usuario atractiva y funcional.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.012.jpeg)

*Se muestra como se ve nuestro sistema de ventas ya ejecut�ndolo.*

####**�Login�**

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.013.png)

####**"Sistema de pr�stamos**�

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.014.png)

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.015.png)

####**Controlador:**

*El controlador act�a como intermediario entre el modelo y la vista, gestionando las interacciones del usuario y actualizando el modelo en consecuencia. Se encarga de interpretar las acciones del usuario, invocar las operaciones adecuadas en el modelo y actualizar la vista correspondiente. Esta separaci�n de responsabilidades permite una mayor flexibilidad en el manejo de eventos y una f�cil integraci�n de nuevas funcionalidades sin afectar la estructura existente.*

*La implementaci�n del patr�n MVC conlleva una serie de beneficios significativos para el desarrollo de software. Entre ellos se incluyen una mejor organizaci�n del c�digo, una mayor modularidad y reutilizaci�n, una facilidad de mantenimiento y evoluci�n, y una mayor escalabilidad y adaptabilidad a medida que los requisitos cambian.*

####**loginControlador.php**

*Este controlador gestiona el inicio de sesi�n, el cierre de sesi�n y la forzada cierre de sesi�n del usuario en el sistema, garantizando la seguridad y la integridad de los datos del usuario.*

####**usuarioControlador.php**

*El c�digo PHP proporcionado define una clase llamada usuarioControlador que extiende la clase usuarioModelo. Esta clase contiene varios m�todos para controlar las operaciones relacionadas con los usuarios en un sistema. Por ejemplo, el m�todo agregar\_usuario\_controlador() valida y agrega un nuevo usuario a la base de datos, mientras que el m�todo eliminar\_usuario\_controlador() gestiona la eliminaci�n de usuarios. Otros m�todos se encargan de actualizar los datos de un usuario, paginar la lista de usuarios y recuperar informaci�n espec�fica de un usuario. El c�digo tambi�n utiliza funciones de validaci�n para garantizar la integridad de los datos antes de realizar operaciones en la base de datos, y utiliza JSON para manejar las respuestas y alertas del sistema de forma din�mica.*

####**vistasControlador.php**

*Este c�digo PHP define la clase **vistasControlador**, que extiende otra clase llamada **vistasModelo**. Dos m�todos principales son definidos: **obtener\_plantilla\_controlador()** devuelve la ruta a la plantilla principal del sitio, mientras que **obtener\_vistas\_controlador()** determina qu� vista cargar seg�n la URL proporcionada. Si se especifica una vista en la URL, se obtiene utilizando el m�todo correspondiente del modelo; de lo contrario, se carga la vista predeterminada "login".*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.016.jpeg)

####**Diagrama de casos de uso**

*Este diagrama de casos de uso muestra el modelo l�gico de los datos de un sistema.*

![](Aspose.Words.9d310a66-e3c3-49fb-b132-20ea124bc805.017.png)

#### ------------------------------------------------------------------

####**Conclusiones**

*En conclusi�n, el Modelo-Vista-Controlador es un enfoque fundamental en el desarrollo de software moderno. Al separar las preocupaciones de datos, presentaci�n y control, MVC promueve una arquitectura m�s limpia, modular y f�cil de mantener. Su adopci�n puede resultar en un c�digo m�s robusto, escalable y flexible, lo que a su vez contribuye a la eficiencia y el �xito a largo plazo de los proyectos de software. Con su capacidad para adaptarse a una amplia gama de aplicaciones y contextos, el patr�n MVC contin�a siendo una herramienta invaluable para los desarrolladores en la creaci�n de aplicaciones de alta calidad y rendimiento.*

#### ------------------------------------------------------------------

 ####**Referencias**

1. *Alvarez, M. A. (20 de Septiembre de 2023). *Desarrollo Web*. Recuperado el 19 de Marzo de 2024, de Qu� es MVC: https://desarrolloweb.com/articulos/que-es-mvc.html*

2. *AppMaster. (07 de Septiembre de 2023). Recuperado el 19 de Marzo de 2024, de Modelo-Vista-Controlador (MVC): https://appmaster.io/es/glossary/modelo-vista-controlador-mvc-es*
3. *Developer Mozilla. (13 de Noviembre de 2023). Recuperado el 19 de Marzo de 2024, de MVC: https://developer.mozilla.org/es/docs/Glossary/MVC*

4. *Francisco J. Vera-Garcia, J. M. (1 de Febrero de 2010). *Journal of Electromyography and Kinesiology*. Recuperado el 19 de Marzo de 2024, de MVC techniques to normalize trunk muscle EMG in healthy women: https://www.sciencedirect.com/science/article/abs/pii/S1050641109000571*
5. *Hern�ndez, U. (Ed.). (22 de Febrero de 2015). *Codigo Facilito*. Recuperado el 19 de Marzo de 2024, de MVC (Model, View, Controller) explicado: https://codigofacilito.com/articulos/mvc-model-view-controller-explicado*


