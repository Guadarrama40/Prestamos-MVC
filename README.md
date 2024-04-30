Castillo Guadarrama Brenda
<br>
Flores Alvarado Julio Cesar
<br><br>
<hr>
Ensayo de un Modelo-Vista-Controlador<br>
Instituto Tecnológico de Tláhuac<br>
Ingeniería en Sistemas Computacionales<br>
Grupo: 8S2. Programación Web PHP con MVC<br>
21 de marzo de 2024<br>
Índice <br>
Resumen	1<br>
Introducción	1<br>
Desarrollo	1<br>
Conclusiones	12 <br>
Referencias	13 <br>


Resumen<br>
El Modelo-Vista-Controlador (MVC) es un patrón arquitectónico ampliamente utilizado en el desarrollo de software. Este enfoque divide una aplicación en tres componentes principales: el modelo, que representa los datos y la lógica de negocio; la vista, que se encarga de la presentación de la información al usuario; y el controlador, que actúa como intermediario entre el modelo y la vista. Este ensayo explora la importancia del MVC en el desarrollo de software moderno, sus beneficios y su aplicación en diferentes contextos.

Introducción<br>
En el panorama actual del desarrollo de software, el modularidad, la escalabilidad y la mantenibilidad son aspectos cruciales para el éxito de un proyecto. El patrón MVC surge como una solución elegante para abordar estos desafíos al promover la separación de preocupaciones y la organización estructurada del código. Al dividir una aplicación en tres componentes distintos pero interconectados, MVC permite un desarrollo más ordenado, facilita la reutilización de código y promueve una mayor flexibilidad y adaptabilidad a medida que los requerimientos evolucionan.

Ejecución del Programa<br>

Para ejecutar este sistema se debe de ingresar a la carpeta de xampp<br>
![WhatsApp Image 2024-04-29 at 6 13 33 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/45a2641a-65cf-4c6d-8348-ed7b230db93d)

Despues ingresar a la carpeta htdocs ya que es el directorio raíz predeterminado donde se almacenan los archivos que constituyen el contenido de un sitio web<br>
![WhatsApp Image 2024-04-29 at 6 14 14 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/db897bf7-c11d-47b1-91a7-2e454c905a38)

Se pega el proyecto de prestamos <br>
![WhatsApp Image 2024-04-29 at 6 14 52 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/9164c438-a131-4831-ba63-3a6f5d067998)

podemos ver que todos los archivos se encuentran en la carpeta documentos <br>
![WhatsApp Image 2024-04-29 at 6 15 20 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/f5e8b22b-ea00-4312-9109-aac87d582094)

Ingresamos a http://localhost/phpmyadmin/ para crear la base de datos<br>
![WhatsApp Image 2024-04-29 at 6 24 39 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/458cacbf-9c28-4957-ac92-e8a822ab00ee)

Importamos el archivo sql donde se encuentra en la carpeta DB<br>
![WhatsApp Image 2024-04-29 at 6 23 11 PM](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/3a4d0dac-265c-445b-bc5b-5382299569d2)



Ingresamos a la url http://localhost/Prestamos/
![WhatsApp Image 2024-04-29 at 6 27 40 PM (1)](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/d23c4d69-8e9e-429d-b40f-4efa41e83fec)

insertamos el usuario: Administrador y contraseña: Administrador
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/78466e31-8c9d-41f4-a1a1-e75fdb2ba063)

Y como se vizualiza esta funcionando el sistema<br>


Desarrollo<br>
Estos archivos son utilizados para crear una página web con funcionalidades básicas como la estructura de la cuadrícula, botones, formularios, barras de desplazamiento, alertas, ventanas emergentes y más. También se utilizan para aplicar estilos a la página web y mejorar la experiencia del usuario.
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/0f31bc38-3734-4572-a4b4-7ac3d606fa44)

Vista:<br>
La vista es la interfaz de usuario que presenta la información al usuario final de manera comprensible y atractiva. Su principal función es mostrar los datos proporcionados por el modelo y permitir la interacción del usuario con la aplicación. Al separar la lógica de presentación del resto del sistema, la vista facilita la adaptación a diferentes dispositivos y plataformas sin afectar la lógica subyacente.
Index.php
Este código PHP carga la configuración de la aplicación y el controlador de vistas, crea una instancia del controlador de vistas y llama a un método en ese controlador para obtener y renderizar la plantilla principal de la aplicación.
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/0b88fa47-6048-4fbf-8250-e723d7ba5c8a)

.htacces<br>
Reescribe cualquier solicitud de URL que consista en letras, números, barras inclinadas, o los caracteres ñ, Ñ, o -, a index.php, pasando el valor capturado como un parámetro views. Por ejemplo, una solicitud a mi_pagina se reescribiría internamente como index.php?views=mi_pagina.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/9757f94d-e2bc-408d-a4ed-ee8d4aa48690)

Plantilla.php<br>
Este código HTML con incrustaciones de PHP establece la estructura básica de una página web dinámica. Incluye un encabezado con metadatos y un título obtenido de una constante PHP. Se carga un archivo PHP para enlaces externos. El cuerpo del documento contiene lógica condicional en PHP para gestionar qué contenido mostrar, dependiendo de la solicitud. Se verifica la existencia de variables de sesión y se redirecciona al inicio de sesión si es necesario. La página principal incluye una barra lateral de navegación y el contenido principal se carga dinámicamente según la vista solicitada. Finalmente, se incluyen archivos PHP adicionales para manejar el cierre de sesión y se cargan scripts necesarios para la funcionalidad de la página.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/2f55cbb5-4f36-4cf2-967b-b34ba0b966d3)
NavBar.php<br>
Este código HTML representa una barra de navegación con tres enlaces. El primer enlace activa/desactiva una barra lateral de navegación. El segundo enlace lleva a una página de actualización de usuario, con la URL construida dinámicamente usando PHP para incluir el ID de sesión cifrado. El tercer enlace parece ser un botón de cierre de sesión.
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/d69f6e51-9aaa-4252-90c5-7274b2071ba0)

NavLateral.php<br>
Este bloque de código HTML con incrustaciones de PHP describe la estructura de una barra de navegación lateral utilizada en una aplicación web. Está compuesto por dos elementos principales dentro de un contenedor <section>. Primero, un fondo oscuro transparente que se muestra cuando la barra lateral está activa, y luego el contenido real de la barra lateral, que incluye un avatar de usuario, una barra de separación y un menú de navegación. Este menú de navegación contiene una lista de elementos de menú representados por enlaces, generados dinámicamente utilizando PHP para construir las URL. Algunos elementos de menú pueden estar condicionados según el nivel de privilegio del usuario, mostrando ciertas opciones de menú solo para usuarios con privilegios específicos.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/0312d746-51b6-440e-bb91-28f6c43c6a77)

Script.php<br>
Describe la inclusión de varios archivos JavaScript en una página web. Los archivos incluidos son principalmente bibliotecas y scripts personalizados esenciales para la funcionalidad y el diseño de la página. Esto incluye bibliotecas como jQuery, Popper, Bootstrap, y Bootstrap Material Design, que proporcionan funcionalidades como manipulación del DOM, posicionamiento de elementos emergentes, estilos y componentes de interfaz de usuario. Además, se incluyen scripts personalizados como main.js y alertas.js, que pueden proporcionar funcionalidades específicas y personalizadas para la página web.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/fdaa6054-2de9-4bf3-ba23-3f6bbe30a1c3)

LogOut.php<br>
Este script implementa la funcionalidad de salida del sistema al hacer clic en un botón específico. Utiliza SweetAlert para mostrar un cuadro de diálogo de confirmación. Si el usuario confirma la salida, se envía una solicitud AJAX al servidor para cerrar la sesión del usuario actual. La solicitud incluye el token de sesión y el nombre de usuario cifrados para garantizar la seguridad de la operación. Una vez completada la solicitud, se procesa la respuesta del servidor, probablemente mostrando alertas o notificaciones al usuario. En resumen, este sistema proporciona una forma segura y controlada para que los usuarios salgan del sistema.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/2aed66ba-8e76-4f58-a821-7b7f499381f1)

Link.php<br>
Describe la inclusión de varios archivos CSS y JavaScript en una página web. Los archivos incluidos proporcionan estilos y funcionalidades para la interfaz de usuario de la página. Esto incluye estilos de normalización (normalize.css), estilos y componentes de Bootstrap (bootstrap.min.css), estilos de diseño de material de Bootstrap (bootstrap-material-design.min.css), iconos de Font Awesome (all.css), estilos para alertas personalizadas (sweetalert2.min.css), y estilos para barras de desplazamiento personalizadas (jquery.mCustomScrollbar.css). Además, se incluye un archivo JavaScript para las alertas personalizadas (sweetalert2.min.js). Estos archivos ayudan a establecer la apariencia y el comportamiento deseado de la página web.
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/35edde4d-341f-44e8-a87b-3f77f7b7f55b)


El sistema de préstamos cuenta con una serie de archivos de vista en el directorio "vistas". Cada archivo .php en este directorio representa una vista específica dentro del sistema, desde la visualización de clientes y ítems hasta la gestión de reservas y usuarios. Estas vistas proporcionan una interfaz para realizar diversas acciones, como agregar nuevos clientes o buscar ítems disponibles.<br>

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/2ee678bb-71f6-449a-921e-da187b5b4e71)

Los archivos en la carpeta assets son esenciales para el funcionamiento del sistema de préstamos. Estos archivos proporcionan las imágenes, iconos, JavaScript, CSS y fuentes que se utilizan para crear una interfaz de usuario atractiva y funcional.<br>

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/636a6ebf-de8c-4bec-9019-2efd84f388ce)
Se muestra como se ve nuestro sistema de ventas ya ejecutándolo.<br>
“Login”<br>
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/5eec6c27-99b7-41cc-aa3a-637a54cbb134)

“Sistema de préstamos”<br>
![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/9a07a9dc-8e94-4384-b727-1957f2be6271)

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/62aaf586-17cb-4982-81bc-8cb3f2582e66)

Controlador:<br>
El controlador actúa como intermediario entre el modelo y la vista, gestionando las interacciones del usuario y actualizando el modelo en consecuencia. Se encarga de interpretar las acciones del usuario, invocar las operaciones adecuadas en el modelo y actualizar la vista correspondiente. Esta separación de responsabilidades permite una mayor flexibilidad en el manejo de eventos y una fácil integración de nuevas funcionalidades sin afectar la estructura existente.
La implementación del patrón MVC conlleva una serie de beneficios significativos para el desarrollo de software. Entre ellos se incluyen una mejor organización del código, una mayor modularidad y reutilización, una facilidad de mantenimiento y evolución, y una mayor escalabilidad y adaptabilidad a medida que los requisitos cambian.<br>
loginControlador.php<br>
Este controlador gestiona el inicio de sesión, el cierre de sesión y la forzada cierre de sesión del usuario en el sistema, garantizando la seguridad y la integridad de los datos del usuario.
usuarioControlador.php<br>
El código PHP proporcionado define una clase llamada usuarioControlador que extiende la clase usuarioModelo. Esta clase contiene varios métodos para controlar las operaciones relacionadas con los usuarios en un sistema. Por ejemplo, el método agregar_usuario_controlador() valida y agrega un nuevo usuario a la base de datos, mientras que el método eliminar_usuario_controlador() gestiona la eliminación de usuarios. Otros métodos se encargan de actualizar los datos de un usuario, paginar la lista de usuarios y recuperar información específica de un usuario. El código también utiliza funciones de validación para garantizar la integridad de los datos antes de realizar operaciones en la base de datos, y utiliza JSON para manejar las respuestas y alertas del sistema de forma dinámica.
vistasControlador.php< <br>
Este código PHP define la clase vistasControlador, que extiende otra clase llamada vistasModelo. Dos métodos principales son definidos: obtener_plantilla_controlador() devuelve la ruta a la plantilla principal del sitio, mientras que obtener_vistas_controlador() determina qué vista cargar según la URL proporcionada. Si se especifica una vista en la URL, se obtiene utilizando el método correspondiente del modelo; de lo contrario, se carga la vista predeterminada "login".

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/27c33591-006e-47b4-829e-298dd62f2141)

Diagrama de casos de uso<br>
Este diagrama de casos de uso muestra el modelo lógico de los datos de un sistema.

![image](https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/f57411d8-90e3-4cc3-8bb5-b800e829e229)

Conclusiones<br>
En conclusión, el Modelo-Vista-Controlador es un enfoque fundamental en el desarrollo de software moderno. Al separar las preocupaciones de datos, presentación y control, MVC promueve una arquitectura más limpia, modular y fácil de mantener. Su adopción puede resultar en un código más robusto, escalable y flexible, lo que a su vez contribuye a la eficiencia y el éxito a largo plazo de los proyectos de software. Con su capacidad para adaptarse a una amplia gama de aplicaciones y contextos, el patrón MVC continúa siendo una herramienta invaluable para los desarrolladores en la creación de aplicaciones de alta calidad y rendimiento.

Referencias<br>

1.	Alvarez, M. A. (20 de Septiembre de 2023). Desarrollo Web. Recuperado el 19 de Marzo de 2024, de Qué es MVC: https://desarrolloweb.com/articulos/que-es-mvc.html
2.	AppMaster. (07 de Septiembre de 2023). Recuperado el 19 de Marzo de 2024, de Modelo-Vista-Controlador (MVC): https://appmaster.io/es/glossary/modelo-vista-controlador-mvc-es
3.	Developer Mozilla. (13 de Noviembre de 2023). Recuperado el 19 de Marzo de 2024, de MVC: https://developer.mozilla.org/es/docs/Glossary/MVC
4.	Francisco J. Vera-Garcia, J. M. (1 de Febrero de 2010). Journal of Electromyography and Kinesiology. Recuperado el 19 de Marzo de 2024, de MVC techniques to normalize trunk muscle EMG in healthy women: https://www.sciencedirect.com/science/article/abs/pii/S1050641109000571
5.	Hernández, U. (Ed.). (22 de Febrero de 2015). Codigo Facilito. Recuperado el 19 de Marzo de 2024, de MVC (Model, View, Controller) explicado: https://codigofacilito.com/articulos/mvc-model-view-controller-explicado















