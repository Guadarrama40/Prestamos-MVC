
<div align="center">

# Ensayo de un Modelo-Vista-Controlador

## Instituto Tecnológico de Tláhuac
## Ingeniería en Sistemas Computacionales
## Programación Web PHP con MVC
## Castillo Guadarrama Brenda
## Flores Alvarado Julio Cesar
## Grupo: 8S2
## 02 de mayo de 2024

</div>

# Índice
 
[***Resumen***	1](#_toc161927398)

[***Introducción***	1](#_toc161927399)

[***Desarrollo***	1](#_toc161927400)

[***Conclusiones***	12](#_toc161927401)

[***Referencias***	13](#_toc161927402)


#
# <a name="_toc161876626"></a><a name="_toc161927398"></a>***Resumen***
*El Modelo-Vista-Controlador (MVC) es un patrón arquitectónico ampliamente utilizado en el desarrollo de software. Este enfoque divide una aplicación en tres componentes principales: el modelo, que representa los datos y la lógica de negocio; la vista, que se encarga de la presentación de la información al usuario; y el controlador, que actúa como intermediario entre el modelo y la vista. Este ensayo explora la importancia del MVC en el desarrollo de software moderno, sus beneficios y su aplicación en diferentes contextos.*
# <a name="_toc161876627"></a><a name="_toc161927399"></a>***Introducción***
*En el panorama actual del desarrollo de software, el modularidad, la escalabilidad y la mantenibilidad son aspectos cruciales para el éxito de un proyecto. El patrón MVC surge como una solución elegante para abordar estos desafíos al promover la separación de preocupaciones y la organización estructurada del código. Al dividir una aplicación en tres componentes distintos pero interconectados, MVC permite un desarrollo más ordenado, facilita la reutilización de código y promueve una mayor flexibilidad y adaptabilidad a medida que los requerimientos evolucionan.*
# <a name="_toc161876628"></a><a name="_toc161927400"></a>***Ejecución del programa***
Paso 1: Se accede a la carpeta XAMPP, un componente fundamental para la instalación y operación eficiente del software XAMPP.

<center><figure>
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/910b667c-073c-446b-91c7-d01041bb9370">
</figure></center><br>
<center><figcaption><i><b>Figura 1:Representación visual del proceso</b></i></figcaption></center><br><br><br><br>

Paso 2: Posteriormente, se navega hacia la carpeta htdocs, una ubicación dentro de la instalación de XAMPP designada para el almacenamiento de los archivos de los sitios web.<br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/e9d19e14-2778-4881-a5c3-9a9147983988">
    <br><figcaption><i><b>Figura 2:Ilustración del procedimiento mencionado</b></i></figcaption>
</figure><br><br><br><br>

Paso 3: Al ingresar a htdcs se crea una carpeta llamada "Prestamos" como se visualiza en la figura 3 <br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/b41c601d-c1a9-4840-9ded-16dc71a446e3)">
    <br><figcaption><i><b>Figura 3:Creación de Carpeta "Prestamos" en htdcs</b></i></figcaption>
</figure><br><br><br><br>

Paso 4: Copiamos los archivos en la carpeta "PRESTAMOS" visualizar en la figura 4 <br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/a16d5d8c-1cef-4d78-8b07-a9fd166b4a60)">
    <br><figcaption><i><b>Figura 4: Copia de Archivos en Carpeta "PRESTAMOS"</b></i></figcaption>
</figure><br><br><br><br>

Paso 5: Entramos a la URL: http://localhost/phpmyadmin/ para crear nuestra base de datos con el nombre de "prestamos", las configuraciones generales de "utf8mb4_spanish2_c1". Y en la base de datos que creamos importamos el archivo spm que se encuentra en la carpeta DB de prestamos como se visualiza en la figura 5 <br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/59111298-e613-4e47-96ec-ada6382122ff" style="width: 800px; height: auto;">
    <br>
    <figcaption><i><b>Figura 5: Importación de Archivo spm en phpMyAdmin</b></i></figcaption>
</figure><br><br><br><br>

Paso 6: Ingresamos a la URL: http://localhost/Prestamos/ y vemos que entramos a la vista principal de prestamos como se visualiza en la figura 6 e ingresamos las contraseñas "Administrador" "Administrador" <br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/373b02ac-1d11-45ee-8ff0-c1e2bb5d7525" style="width: 800px; height: auto;">
    <br><figcaption><i><b>Figura 6: Vista Principal de Prestamos con Contraseñas</b></i></figcaption>
</figure><br><br><br><br>

Paso 7: Pagina principal de prestamos <br>
<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/a59543ec-88d7-4324-a248-3a5b2dcccf99" style="width: 800px; height: auto;">
    <br><figcaption><i><b>Figura 7: Página Principal de Prestamos</b></i></figcaption>
</figure><br><br><br><br>


# <a name="_toc161876628"></a><a name="_toc161927400"></a>***Desarrollo***
Estos archivos son utilizados para crear una página web con funcionalidades básicas como la estructura de la cuadrícula, botones, formularios, barras de desplazamiento, alertas, ventanas emergentes y más. También se utilizan para aplicar estilos a la página web y mejorar la experiencia del usuario.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/38c611bc-2460-498a-8d9b-e3d52f079c9b" alt="imagen" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 8: Archivos de diseño</b></i></figcaption><br><br><br><br>
</figure>
El Modelo-Vista-Controlador se compone de tres elementos clave:

## <a name="_toc161876629"></a>***Modelo:***
*El modelo representa los datos subyacentes de la aplicación y la lógica de negocio asociada. Es responsable de manejar la manipulación y el almacenamiento de los datos, así como de aplicar las reglas de negocio necesarias para procesarlos correctamente. Al separar la lógica de negocio del resto de la aplicación, el modelo facilita la reutilización y la prueba de la funcionalidad de manera independiente.*

**LoginModelo.php**

Define una clase loginModelo que extiende otra clase llamada mainModel, indicando que probablemente herede funcionalidades relacionadas con la interacción con la base de datos. Dentro de esta clase, hay un método protegido llamado iniciar\_sesion\_modelo($datos), que se encarga de iniciar sesión en el sistema. Este método ejecuta una consulta SQL preparada para seleccionar los datos de usuario correspondientes a las credenciales proporcionadas. El resultado de la consulta se devuelve para su posterior procesamiento, como verificar si las credenciales son válidas.

**mainModel.php**

Esta clase proporciona una serie de funciones esenciales para realizar operaciones comunes en un sistema, como interactuar con la base de datos, validar datos, encriptar y desencriptar información, y gestionar la paginación de resultados. Esto promueve la reutilización de código y la implementación eficiente de funcionalidades en el sistema.

**usuarioModelo.php**

Estos métodos ofrecen una interfaz para realizar operaciones comunes de CRUD (Crear, Leer, Actualizar, Eliminar) en la tabla de usuarios, promoviendo la modularidad y reutilización del código.

**vistasModelo.php**

Este código determina la vista que se debe cargar en función de la solicitud del usuario, asegurando que solo se acceda a vistas permitidas y manejando adecuadamente los casos donde la vista solicitada no existe.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/04eff6d5-c053-4eaf-ab7b-506976cae1a1" alt="imagen" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 9: Archivo de vistasModelo.php</b></i></figcaption><br><br><br><br>
</figure>

## <a name="_toc161876630"></a>***Vista:***
*La vista es la interfaz de usuario que presenta la información al usuario final de manera comprensible y atractiva. Su principal función es mostrar los datos proporcionados por el modelo y permitir la interacción del usuario con la aplicación. Al separar la lógica de presentación del resto del sistema, la vista facilita la adaptación a diferentes dispositivos y plataformas sin afectar la lógica subyacente.*

**Index.php**

Este código PHP carga la configuración de la aplicación y el controlador de vistas, crea una instancia del controlador de vistas y llama a un método en ese controlador para obtener y renderizar la plantilla principal de la aplicación.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/2dde8ade-f0ce-452c-9e3e-62a5a1503f51" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 10: Código de Index.php</b></i></figcaption><br><br><br><br>
</figure>



**.htacces**

Reescribe cualquier solicitud de URL que consista en letras, números, barras inclinadas, o los caracteres ñ, Ñ, o -, a index.php, pasando el valor capturado como un parámetro views. Por ejemplo, una solicitud a mi\_pagina se reescribiría internamente como index.php?views=mi\_pagina.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/d2b6664f-d6ba-4c8f-a572-e952bcc43a39" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 11: Código de .htacces.php</b></i></figcaption><br><br><br><br>
</figure>



**Plantilla.php**

Este código HTML con incrustaciones de PHP establece la estructura básica de una página web dinámica. Incluye un encabezado con metadatos y un título obtenido de una constante PHP. Se carga un archivo PHP para enlaces externos. El cuerpo del documento contiene lógica condicional en PHP para gestionar qué contenido mostrar, dependiendo de la solicitud. Se verifica la existencia de variables de sesión y se redirecciona al inicio de sesión si es necesario. La página principal incluye una barra lateral de navegación y el contenido principal se carga dinámicamente según la vista solicitada. Finalmente, se incluyen archivos PHP adicionales para manejar el cierre de sesión y se cargan scripts necesarios para la funcionalidad de la página.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/6df877a6-c8f8-44b4-9878-629f81e466e4" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 12: Código de plantilla.php</b></i></figcaption><br><br><br><br>
</figure>


**NavBar.php**

Este código HTML representa una barra de navegación con tres enlaces. El primer enlace activa/desactiva una barra lateral de navegación. El segundo enlace lleva a una página de actualización de usuario, con la URL construida dinámicamente usando PHP para incluir el ID de sesión cifrado. El tercer enlace parece ser un botón de cierre de sesión.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/248d3b18-1923-4c06-9838-b60fbcbeef57" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 13: Código de NavBar.php</b></i></figcaption><br><br><br><br>
</figure>




**NavLateral.php**
Este bloque de código HTML con incrustaciones de PHP describe la estructura de una barra de navegación lateral utilizada en una aplicación web. Está compuesto por dos elementos principales dentro de un contenedor <section>. Primero, un fondo oscuro transparente que se muestra cuando la barra lateral está activa, y luego el contenido real de la barra lateral, que incluye un avatar de usuario, una barra de separación y un menú de navegación. Este menú de navegación contiene una lista de elementos de menú representados por enlaces, generados dinámicamente utilizando PHP para construir las URL. Algunos elementos de menú pueden estar condicionados según el nivel de privilegio del usuario, mostrando ciertas opciones de menú solo para usuarios con privilegios específicos.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/3b94ee31-221a-493d-b88b-8012a5f227a2" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 14: Código de NavLateral.php</b></i></figcaption><br><br><br><br>
</figure>

**Script.php**

Describe la inclusión de varios archivos JavaScript en una página web. Los archivos incluidos son principalmente bibliotecas y scripts personalizados esenciales para la funcionalidad y el diseño de la página. Esto incluye bibliotecas como jQuery, Popper, Bootstrap, y Bootstrap Material Design, que proporcionan funcionalidades como manipulación del DOM, posicionamiento de elementos emergentes, estilos y componentes de interfaz de usuario. Además, se incluyen scripts personalizados como **main.js** y **alertas.js**, que pueden proporcionar funcionalidades específicas y personalizadas para la página web.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/7ed74d65-e8a3-4351-be02-d7a437074eb9" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 15: Código de Script.php</b></i></figcaption><br><br><br><br>
</figure>


**LogOut.php**

Este script implementa la funcionalidad de salida del sistema al hacer clic en un botón específico. Utiliza SweetAlert para mostrar un cuadro de diálogo de confirmación. Si el usuario confirma la salida, se envía una solicitud AJAX al servidor para cerrar la sesión del usuario actual. La solicitud incluye el token de sesión y el nombre de usuario cifrados para garantizar la seguridad de la operación. Una vez completada la solicitud, se procesa la respuesta del servidor, probablemente mostrando alertas o notificaciones al usuario. En resumen, este sistema proporciona una forma segura y controlada para que los usuarios salgan del sistema.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/46d6a193-7bbc-4647-a884-db7e12388090" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 16: Código de LogOut.php</b></i></figcaption><br><br><br><br>
</figure>

**Link.php**

Describe la inclusión de varios archivos CSS y JavaScript en una página web. Los archivos incluidos proporcionan estilos y funcionalidades para la interfaz de usuario de la página. Esto incluye estilos de normalización (**normalize.css**), estilos y componentes de Bootstrap (**bootstrap.min.css**), estilos de diseño de material de Bootstrap (**bootstrap-material-design.min.css**), iconos de Font Awesome (**all.css**), estilos para alertas personalizadas (**sweetalert2.min.css**), y estilos para barras de desplazamiento personalizadas (**jquery.mCustomScrollbar.css**). Además, se incluye un archivo JavaScript para las alertas personalizadas (**sweetalert2.min.js**). Estos archivos ayudan a establecer la apariencia y el comportamiento deseado de la página web.


<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/cb5e913d-fbee-4af9-ac94-340f0eb0d0a8" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 17: Código de Link.php</b></i></figcaption><br><br><br><br>
</figure>







El sistema de préstamos cuenta con una serie de archivos de vista en el directorio "vistas". Cada archivo .php en este directorio representa una vista específica dentro del sistema, desde la visualización de clientes y ítems hasta la gestión de reservas y usuarios. Estas vistas proporcionan una interfaz para realizar diversas acciones, como agregar nuevos clientes o buscar ítems disponibles.


<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/b5e757bd-ba82-40b7-ac84-e452a0497cba" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 18: Archivos de vistas</b></i></figcaption><br><br><br><br>
</figure>



Los archivos en la carpeta assets son esenciales para el funcionamiento del sistema de préstamos. Estos archivos proporcionan las imágenes, iconos, JavaScript, CSS y fuentes que se utilizan para crear una interfaz de usuario atractiva y funcional.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/364eb7cd-5019-491b-a93c-3254e2533870" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 19: Carpeta assets </b></i></figcaption><br><br><br><br>
</figure>


Se muestra como se ve nuestro sistema de ventas ya ejecutándolo.

**“Login”**

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/5bfe3ca5-6e3d-49e4-bb1a-cd5ae54527c5" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 20: Login </b></i></figcaption><br><br><br><br>
</figure>






“Sistema de préstamos”

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/5ef8fb9f-5c49-4ed0-b427-1d7783746aaa" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 20: Prestamos Home </b></i></figcaption><br><br><br><br>

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/9d26e659-bae3-4be6-91ae-2c6217eff464" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 21: Prestamos/ Cliente </b></i></figcaption><br><br><br><br>
</figure>

## <a name="_toc161876631"></a>***Controlador:***
*El controlador actúa como intermediario entre el modelo y la vista, gestionando las interacciones del usuario y actualizando el modelo en consecuencia. Se encarga de interpretar las acciones del usuario, invocar las operaciones adecuadas en el modelo y actualizar la vista correspondiente. Esta separación de responsabilidades permite una mayor flexibilidad en el manejo de eventos y una fácil integración de nuevas funcionalidades sin afectar la estructura existente.*

*La implementación del patrón MVC conlleva una serie de beneficios significativos para el desarrollo de software. Entre ellos se incluyen una mejor organización del código, una mayor modularidad y reutilización, una facilidad de mantenimiento y evolución, y una mayor escalabilidad y adaptabilidad a medida que los requisitos cambian.*

**loginControlador.php**

Este controlador gestiona el inicio de sesión, el cierre de sesión y la forzada cierre de sesión del usuario en el sistema, garantizando la seguridad y la integridad de los datos del usuario.

**usuarioControlador.php**

El código PHP proporcionado define una clase llamada usuarioControlador que extiende la clase usuarioModelo. Esta clase contiene varios métodos para controlar las operaciones relacionadas con los usuarios en un sistema. Por ejemplo, el método agregar\_usuario\_controlador() valida y agrega un nuevo usuario a la base de datos, mientras que el método eliminar\_usuario\_controlador() gestiona la eliminación de usuarios. Otros métodos se encargan de actualizar los datos de un usuario, paginar la lista de usuarios y recuperar información específica de un usuario. El código también utiliza funciones de validación para garantizar la integridad de los datos antes de realizar operaciones en la base de datos, y utiliza JSON para manejar las respuestas y alertas del sistema de forma dinámica.

**vistasControlador.php<**

Este código PHP define la clase **vistasControlador**, que extiende otra clase llamada **vistasModelo**. Dos métodos principales son definidos: **obtener\_plantilla\_controlador()** devuelve la ruta a la plantilla principal del sitio, mientras que **obtener\_vistas\_controlador()** determina qué vista cargar según la URL proporcionada. Si se especifica una vista en la URL, se obtiene utilizando el método correspondiente del modelo; de lo contrario, se carga la vista predeterminada "login".

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/48e66681-5a40-4fdc-9c54-550a1b2d2c56" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 22: Archivo VistasControlador.php</b></i></figcaption><br><br><br><br>
</figure>

## ***Diagrama de casos de uso***
Este diagrama de casos de uso muestra el modelo lógico de los datos de un sistema.

<figure style="text-align: center;">
    <img src="https://github.com/hjdzsklfj/Prestamos-MVC/assets/150282544/48e66681-5a40-4fdc-9c54-550a1b2d2c56" style="width: 800px; height: auto;">
     <br><figcaption><i><b>Figura 23: Diagrama de caso de uso </b></i></figcaption><br><br><br><br>
</figure>

# <a name="_toc161876632"></a><a name="_toc161927401"></a>***Conclusiones***
*En conclusión, el Modelo-Vista-Controlador es un enfoque fundamental en el desarrollo de software moderno. Al separar las preocupaciones de datos, presentación y control, MVC promueve una arquitectura más limpia, modular y fácil de mantener. Su adopción puede resultar en un código más robusto, escalable y flexible, lo que a su vez contribuye a la eficiencia y el éxito a largo plazo de los proyectos de software. Con su capacidad para adaptarse a una amplia gama de aplicaciones y contextos, el patrón MVC continúa siendo una herramienta invaluable para los desarrolladores en la creación de aplicaciones de alta calidad y rendimiento.*

# <a name="_toc161876633"></a><a name="_toc161927402"></a>***Referencias***
#
1. Alvarez, M. A. (20 de Septiembre de 2023). *Desarrollo Web*. Recuperado el 19 de Marzo de 2024, de Qué es MVC: https://desarrolloweb.com/articulos/que-es-mvc.html
1. *AppMaster*. (07 de Septiembre de 2023). Recuperado el 19 de Marzo de 2024, de Modelo-Vista-Controlador (MVC): https://appmaster.io/es/glossary/modelo-vista-controlador-mvc-es
1. *Developer Mozilla*. (13 de Noviembre de 2023). Recuperado el 19 de Marzo de 2024, de MVC: https://developer.mozilla.org/es/docs/Glossary/MVC
1. Francisco J. Vera-Garcia, J. M. (1 de Febrero de 2010). *Journal of Electromyography and Kinesiology*. Recuperado el 19 de Marzo de 2024, de MVC techniques to normalize trunk muscle EMG in healthy women: https://www.sciencedirect.com/science/article/abs/pii/S1050641109000571
1. Hernández, U. (Ed.). (22 de Febrero de 2015). *Codigo Facilito*. Recuperado el 19 de Marzo de 2024, de MVC (Model, View, Controller) explicado: https://codigofacilito.com/articulos/mvc-model-view-controller-explicado



