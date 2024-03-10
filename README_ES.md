<p align="right">
	<a href="README.md">Click here for English version</a>
</p>

# TaskTeam 👨🏽‍💻

TaskTeam es el proyecto final para mi Certificado de Educación Superior en Desarrollo de Aplicaciones Web. Es un sistema de gestión de tareas web que permite la organización y seguimiento eficiente de las tareas de los empleados dentro de una organización. Cuenta con una interfaz intuitiva para el usuario y está formada por dos componentes principales: un módulo de gestión de empleados y un módulo de gestión de tareas.

El módulo de gestión de empleados permite el registro, visualización, edición y eliminación de empleados. Incluye campos para detalles como nombres, cargos y departamentos.

El módulo de gestión de tareas permite la creación, asignación y gestión de tareas asociadas con los empleados. Las tareas pueden ser buscadas, filtradas y ordenadas según diversos criterios. Cada tarea está vinculada a un empleado específico e incluye detalles como descripción de la tarea, fechas de inicio y fin, y estado. Este módulo proporciona una visión general de las tareas asignadas a cada empleado, facilitando la distribución y seguimiento efectivos de las tareas.

El sistema cuenta con una interfaz intuitiva y amigable para el usuario, ofreciendo un inicio de sesión de acceso diferente para empleados o jefes de departamento, formularios de registro y edición de empleados, así como una sección dedicada a la gestión de tareas. Tanto los empleados como las tareas pueden ser buscados y filtrados por diferentes criterios, facilitando su ubicación y seguimiento. Además, se proporciona la posibilidad de asignar tareas a empleados específicos, registrar la fecha de inicio y fin de cada tarea y ver un resumen general de las tareas asignadas a cada empleado.

TaskTeam está desarrollado utilizando tecnologías web como HTML, CSS, JavaScript, Bootstrap, PHP y MySQL, con el objetivo de crear una aplicación robusta y funcional. Además, se aplican buenas prácticas de diseño y programación.

En resumen, esta aplicación web tiene como objetivo proporcionar una solución integral y eficiente para la gestión de empleados y tareas, permitiendo a las empresas mejorar su organización interna, aumentar la productividad y optimizar el seguimiento de las tareas asignadas a su personal.

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Estado%20del%20Proyecto-Finalizado-brightgreen"/>
</p>

<br>

## Índice

- [Instalación](#instalación)
- [Modelo de Desarrollo](#modelo-de-desarrollo)
- [Tecnologías empleadas](#tecnologías)
- [Funcionalidades](#funcionalidades)
- [Base de Datos](#base-de-datos)
- [Backend](#back-end)
  incluir diagrama de clases
- [Frontend](#front-end)
- [Estructura de Archivos](#estructura-de-archivos)
- [Capturas](#capturas)
- [Demo](#demo)
- [Licencia](#licencia)
- [Autor](#autor)

<br>

<a name="instalación"></a>

## Instalación

### Requisitos Previos

Asegúraese de tener XAMPP instalado en tu computadora. Puedes descargarlo desde [el sitio web oficial de Apache Friends.](https://www.apachefriends.org/es/index.html)

### Pasos de Instalación

- **Instalación de XAMPP**:

  - Descarga el instalador de XAMPP desde el sitio web oficial y ejecútalo.
  - Sigue las instrucciones del instalador para completar la instalación de XAMPP en tu computadora.
  - Una vez instalado, abre el Panel de Control de XAMPP y asegúrate de que los servicios de Apache y MySQL estén activos.

- **Configuración de la Base de Datos**:

  - Abre tu navegador web y visita [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
  - Crea una nueva base de datos llamada daw_m12_app.
  - Importa el archivo SQL proporcionado con la aplicación web o crea manualmente las tablas y relaciones necesarias.

- **Transferencia de la Aplicación Web**:

  - Copia los archivos de la aplicación web al directorio htdocs dentro del directorio de instalación de XAMPP. Por lo general, este directorio se encuentra en C:\xampp\htdocs en sistemas Windows o /Applications/XAMPP/htdocs en macOS. La ruta resultante debería ser: /Applications/XAMPP/xamppfiles/htdocs/DAW_FP/M12_WebApp/.

- **Iniciar el Servidor Local**:

  - Vuelve al Panel de Control de XAMPP y haz clic en "Start" para iniciar los servicios de Apache y MySQL.
  - Abre tu navegador web y visita [http://localhost/DAW_FP/M12_WebApp/index_main.php](http://localhost/DAW_FP/M12_WebApp/index_main.php)

- **Pruebas de Aplicación**:
  - Si todo se configuró correctamente, deberías poder ver la página de inicio de sesión de TaskTeam. ¡Felicidades! Has instalado con éxito tu aplicación web PHP en tu servidor local utilizando XAMPP. Ahora puedes comenzar a desarrollar y probar tu aplicación sin necesidad de una conexión a internet.

<br>

<a name="modelo-de-desarrollo"></a>

## Modelo de Desarrollo

Para establecer el ciclo de vida de **TaskTeam**, se ha optado por el modelo en cascada con realimentación. Esta elección se basa tras considerar que este modelo es el más adecuado para el alcance y tamaño del proyecto. Aunque en desarrollos muy grandes puede resultar complicado alcanzar el éxito debido a las numerosas dependencias que se generan, para proyectos más modestos se ha demostrado como uno de los más eficientes debido a su aplicación sencilla.

El modelo en cascada con realimentación consta de una serie de fases que se completan de forma secuencial, pero cada una de ellas puede retroalimentar a la anterior en caso de ser necesario.

Esto puede ocurrir cuando se detecta un error en una fase previa y se corrige, o cuando se produce un cambio en alguna condición del entorno que requiere ajustes.

Las fases marcadas por este modelo se ajustan perfectamente al esquema propuesto en el proyecto, que son: análisis, diseño, codificación y pruebas. A excepción de la fase de mantenimiento, ya que el ciclo de vida de **TaskTeam** no contempla una fase de explotación.

<br>
<div align="center">
  <a>
    <img src="https://github.com/juancumbeq/daw_m12_web_project/blob/main/images/Diagrama_ModeloDesarrollo.png?raw=true" height= "90%" title="Modelo de Desarrollo">
  </a>
</div>

<br>

<a name="tecnologías"></a>

## Tecnologías Utilizadas

En TaskTeam, se han utilizado diversas tecnologías para su desarrollo y funcionamiento. La mayoría de ellas han sido ampliamente utilizadas a lo largo del ciclo de formación. A continuación, se proporciona una breve descripción de para qué se ha utilizado cada una de ellas:

<br>

- **HTML5**: HTML5 se ha utilizado para la estructura y marcado de las páginas web de TaskTeam. Es el lenguaje estándar para crear contenido web y permite definir la estructura de elementos y su interacción.

- **CSS**: Las Hojas de Estilo en Cascada se han utilizado para aplicar estilos y diseños a las páginas de TaskTeam. Permite controlar la presentación visual de elementos, como colores, fuentes, tamaños, disposiciones de página, entre otros. En este proyecto en particular, el uso de CSS viene junto con Bootstrap.

- **Bootstrap**: Bootstrap es un marco de trabajo de código abierto que proporciona un conjunto de herramientas y estilos CSS predefinidos, permitiendo la construcción rápida y fácil de interfaces web receptivas y atractivas. Se ha utilizado en la aplicación para facilitar la creación de una interfaz de usuario moderna y adaptable.

- **JavaScript**: JavaScript se ha utilizado para implementar interactividad en las páginas de TaskTeam, permitiendo así acciones dinámicas para y por el usuario. Más específicamente, he utilizado:

- **SweetAlert2**: Es una biblioteca de JavaScript utilizada para crear ventanas emergentes y notificaciones personalizadas al intentar realizar una modificación en un registro de base de datos. Proporciona una experiencia de usuario mejorada al mostrar mensajes de manera atractiva y de forma amigable.

- **DataTables**: DataTables es una biblioteca de JavaScript utilizada en TaskTeam para mejorar la visualización y manipulación de tablas de datos. Proporciona características avanzadas como paginación, filtrado, ordenación y búsqueda en tablas, mejorando la usabilidad y presentación de información tabular en la aplicación. Inicialmente, DataTables se creó como una biblioteca de jQuery, lo que significa que requería incluir la biblioteca de jQuery en la página web. Sin embargo, en versiones más recientes, DataTables también puede utilizarse sin jQuery como una biblioteca de JavaScript independiente, aunque se mantiene la sintaxis de jQuery.

- **PHP**: Se ha utilizado como el lenguaje de programación del lado del servidor en TaskTeam. Permite realizar operaciones y lógica comerciales, acceder y administrar bases de datos y generar contenido dinámico en páginas web. La ejecución de archivos ".php" se ha realizado en XAMPP ya que cuenta con un intérprete del lado del servidor en Apache.

- **XAMPP**: Es un paquete de software que incluye un servidor web Apache, una base de datos MySQL y el intérprete PHP. Se ha utilizado para crear un entorno de desarrollo local en el que se ha ejecutado y probado TaskTeam.

- **phpMyAdmin**: Para poder acceder a la base de datos MySQL, es necesario contar con un Sistema de Gestión de Bases de Datos (DBMS). phpMyAdmin es el DBMS de XAMPP y se ha utilizado en TaskTeam para gestionar la base de datos y realizar operaciones como crear tablas, consultas y modificaciones a los datos.

- **Navegadores**: Principalmente, se han utilizado dos navegadores web, Google Chrome y Brave, para probar y verificar el funcionamiento de la aplicación, así como la compatibilidad y el rendimiento en diferentes entornos de visualización.

- **Visual Studio Code**: Es un editor de código de Microsoft utilizado para escribir y editar archivos HTML, JavaScript y PHP. Proporciona herramientas y extensiones que facilitan la programación y mejoran la productividad.

- **ClickUp**: Es una herramienta de gestión de proyectos utilizada para organizar y realizar un seguimiento de las tareas, asignar responsabilidades, establecer plazos y prioridades.

- **Draw.io**: Draw.io es una herramienta de creación de diagramas utilizada para diseñar y representar visualmente la estructura de la base de datos (diagrama E-R, diagrama relacional), diagramas de casos de uso y otros diagramas necesarios para el desarrollo del proyecto.

Cada una de estas tecnologías ha desempeñado un papel clave en el desarrollo y funcionamiento de TaskTeam, permitiendo la creación de una aplicación web funcional, interactiva y visualmente atractiva.

<br>

<a name="funcionalidades"></a>

## Funcionalidades

- #### Autenticación de Usuario

  - Cada usuario del sistema cuenta con un correo y una contraseña que le permite acceder al aplicativo.

- #### Gestión de Empleados

  - Los managers de cada departamento son los únicos que disponen de permisos para acceder al listado de empleados, mediante este este módulo se permite lo siguiente:
    - Adición de un empleado al sistema mediante formulario.
    - Edición de datos de empleado.
    - Borrado de registro de empleado.
    - Visionado de tareas asignadas a un empleado en concreto.

- #### Gestión de Tareas
  - Los empleados y los managers de departamente tiene acceso a este módulo, sin embargo, las funciones permitidas son limitadas para el caso de los empleados.
  - Permisos de managers de departamento:
    - Adición de tareas correspondientes a un departamento mediante formulario.
    - Edición de datos de tarea.
    - Borrado de registro de tareas.
    - Asignación de tareas a empleados.
  - Permisos de empleados:
    - Edición del estado de la tarea asignada.

<br>

Para conocer en detalle las funcionalidades del aplicativo podemos hacer referencia de los diagramas de casos de uso Los cuales, se emplean para representar los requisitos de la aplicación web desde la perspectiva de los distintos agentes que interactúan con ella, como usuarios, sistemas o aplicaciones externas. En este proyecto en particular, solo los empleados y los jefes de departamento tienen interacción con el aplicativo.

<br>

<p align="center">
    <img src="https://github.com/juancumbeq/daw_m12_web_project/blob/main/images/Diagrama_CasosUsoJefe.png?raw=true" width= "42%"title="Use Cases">&nbsp;&nbsp;&nbsp;
    <img src="https://github.com/juancumbeq/daw_m12_web_project/blob/main/images/Diagrama_CasosUsoEmpleado.png?raw=true" width= "50%"title="Use Cases">
</p>
<br>

<br>

<a name="base-de-datos"></a>

## Base de datos



<p align="center">
    <img src="https://github.com/juancumbeq/daw_m12_web_project/blob/main/images/Diagrama_ER.png?raw=true" width= "90%"title="Use Cases">&nbsp;&nbsp;&nbsp;
</p>

<p align="center">
    <img src="https://github.com/juancumbeq/daw_m12_web_project/blob/main/images/Diagrama_Relacional.png?raw=true" width= "70%"title="Use Cases">
</p>

<br>

<a name="backend"></a>

## Back-end

El desarrollo del Back-end se llevó a cabo siguiendo el patrón MVC. Se han implementado las clases para los controladores y los modelos, definidas en las fase de análisis.
Como se ha mencionado en el apartado de Diagrama se Clases, el procedimiento de implementación del back-end de las partes principales de la aplicación vino como consecuencia de tener estructurado y mínimamente funcional el front-end, porque de esta manera era posible manejar datos reales y conocer el flujo de los mismos, para la detección y solución de errores.
45
TaskTeam - Juan Fernando Cumbe Quispi
Para poder entender con mayor facilidad los detalles de las clases y su métodos, es importante tener en cuenta que los controladores y los modelos llevan a cabo todo el manejo del back-end, el cuál ha sido implementado en PHP. Encargándose el modelo de toda la interacción con la base de datos y el controlador de la recepción, manejo y envío de estos mismos datos hacia y desde el modelo y la vista.
En la codificación de los controladores también se instancian objetos de los modelos correspondientes, conforme se requiera interactuar con la base de datos. De esta manera es únicamente el controlador el que se puede comunicar con el modelo, dotando de una mayor seguridad al aplicativo.
Por último, se codifican las clases del modelo, definiendo todas las consultas requeridas para devolver la información solicitada por el controlador.
A lo largo del desarrollo del back-end se detectaron deficiencias en las clases que se plantearon inicialmente, ya que a medida que iba construyendo la aplicación surgían nuevas necesidades y oportunidades de optimización y reutilización de código. De modo que, durante toda la implementación del código hubo una retroalimentación con el análisis del diagrama de clases, dando como resultado final el que podemos encontrar en el Anexo VI - Diagrama de Clases.
A continuación se mencionan las principales clases que manejan el grueso de los datos del aplicativo:
● Clase LoginController (controlador de acceso): se encarga de recibir las credenciales de usuario procedentes de la vista, usa como propiedades un objeto userModel que le permite establecer conexión con el modelo de usuarios.
○ login(): transmite las credenciales de usuario hacia el modelo, inicia una sesión y una vez obtiene una respuesta por parte del modelo almacena los datos dentro de la variable $\_SESSION. Finalmente redirige al usuario a la página de HOME. En caso de que las credenciales sean erróneas pasa un mensaje a la vista para informar al usuario.
46

TaskTeam - Juan Fernando Cumbe Quispi
47
● Clase UserModel (modelo de usuarios): recibe los datos por parte del controlador LoginController y haciendo uso de la propiedad $conexion puede establecer contacto con la base de datos correspondiente.
○ verificarCredenciales(): inserta las credenciales del usuario dentro de las sentencias SQL que le permiten conocer la identidad del usuario mencionado. Retorna los datos correspondientes en función de los resultados de las querys.
● Clase EmployeeController (controlador de los empleados de un departamento): es el encargado de gestionar el CRUD de empleados, es decir, se encarga de la lectura, creación, actualizado y borrado de empleados. Es necesario disponer de permisos como jefe de departamento para acceder a la vista correspondiente y por ende hacer uso del controlador. Usa como propiedades un objeto employeesModel que le permite establecer conexión con el modelo de empleados.
○ CreateEmployees(): recibe los datos del formulario de la vista dentro de un array y extrae cada uno de los datos, guardándolos en variables que posteriormente enviará al modelo. Si en el modelo no se produce algún error durante el proceso en creado, se redirecciona al usuario hacia la página de la lista de empleados.
○ FixedDataCreateForm(): para crear un nuevo empleado es necesario disponer de información determinada en el formulario, como son los desplegables. Este método se encarga de mediante el identificativo del departamento solicitar la información relevante del mismo, como pueden ser los puestos disponibles para ese departamento.
○ ReadEmployees(): realiza una llamada al método correspondiente del modelo para obtener un array con toda la información de los empleados de la empresa.
○ UpdateEmployees(): funciona de manera similar al método CreateEmployees() pero con la diferencia de que requiere de un parámetro más para funcionar, se trata del identificativo del empleado, lo que le permite indicar al modelo sobre qué registro actuar.

TaskTeam - Juan Fernando Cumbe Quispi
48
○ FixedDataUpdateForm(): del mismo modo que con FixedDataCreateForm(), a la hora de actualizar la información de los empleados es necesario cargar de manera previa información en el formulario.
○ DeleteEmployees(): mediante el uso de un identificador realiza un llamado al método correspondiente del modelo para ejecutar el borrado de un empleado.
● Clase EmployeesModel (modelo de los empleados): es la clase encargada de actuar sobre la BBDD ejecutando las sentencias SQL correspondientes.
○ CreateEmployeesModel(): recibe a través del controlador la información del empleado que necesita ser creado. Se encarga de gestionar el renombrado y copiado de los archivos subidos al formulario para que pasen a estar a disposición del back-end. En caso de que la sentencia de inserción se realice de manera satisfactoria se retorna true.
○ FixedDataCreateFormEmployees(): se encarga de obtener los puestos y la información del departamento, para que a la hora de crear un nuevo empleado se disponga de información seleccionable relevante a cada departamento.
○ ReadEmployees(): extrae toda la información de los empleados de la base de datos y la entrega al controlador.
○ UpdateEmployees(): nuevamente de manera similar al método de creado, se encarga de insertar la nueva información del empleado para actualizar el registro correspondiente. Así mismo, gestiona el borrado de archivos obsoletos de empleados y traslada las versiones actualizadas.
○ FixedDataUpdateFormModel(): haciendo uso del $id_empleado, obtiene toda la información del registro elegido para que en el formulario de actualización de datos aparezcan por defecto los datos actuales y se pueda seleccionar con precisión qué dato editar.
○ DeleteEmployeeModel(): se encarga del borrado del registro y de los archivos relevantes a un empleado en concreto.

TaskTeam - Juan Fernando Cumbe Quispi
49
● Clase TasksController (controlador de las tareas): es el encargado de gestionar el CRUD de las tareas. Los empleados pueden hacer uso de algunos de los métodos de esta clase como son los de lectura y actualizado, pero solo los usuarios con permisos suficientes pueden acceder a los métodos de creación y eliminación de tareas. Usa como propiedades un objeto tasksModel que le permite establecer conexión con el modelo de las tareas.
○ CreateTasks(): se encarga de recibir los datos del formulario dentro de un array y de desestructurarlos en variables independientes que luego envía al modelo para que construya una sentencia SQL y la ejecute. Si durante el proceso no se produce algún error se redirecciona al usuario a la página de la lista de tareas.
○ FixedDataCreateForm(): a la hora de crear una tarea es necesario asignarla a un departamento y un empleado en concreto. Este método se encarga de usar el identificador del departamento para solicitar los datos correspondientes al modelo.
○ ReadTasksDptoGeneral(): método que se encarga de la lectura de todas las tareas correspondientes a un departamento.
○ ReadTasksDptoSpecific(): este método realiza una función similar al anterior con la diferencia de que las tareas que obtiene han de ser las asignadas a un empleado en particular.
○ UpdateTasks(): del mismo modo que el método de creado se encarga de recibir los datos del formulario y desestructurarlos en variables independientes que luego envía al modelo para que construya una sentencia SQL y la ejecute. En caso de que la operación se realice de manera exitosa se redirecciona al usuario hacia la lista de tareas.
○ FixedDataUpdateForm(): se encarga de obtener del modelo toda la información relevante de una tarea para rellenar el formulario de manera predeterminada.
○ DeleteTasks(): haciendo uso del identificador de una tarea, indica al modelo sobre qué registro actuar para ejecutar la operación de borrado.
● Clase TasksModel (modelo de las tareas): ejecuta las sentencias SQL sobre la base de datos correspondiente al CRUD.

TaskTeam - Juan Fernando Cumbe Quispi
○ CreateTasksModel(): recibe los datos del controlador en varios parámetros y los usa en la sentencia SQL de creado de tarea. En caso de que todo se ejecute correctamente retorna true.
○ FixedDataCreateFormModel(): obtiene toda la información relevante del departamento como es la lista de los empleados disponibles.
○ ReadTasksDptoGeneralModel(): obtiene los datos de todas las tareas de un departamento en concreto. Esa información será mostrada posteriormente en forma de tabla.
○ ReadTasksDptoSpecificModel(): se encarga de obtener todos los datos de las tareas de un empleado en particular.
○ UpdateTasks(): de la misma manera que el método de creado, recibe todos los datos que se han de actualizar a través de los parámetros. Cuenta con un parámetro extra que indica sobre qué registro se ha de ejecutar la sentencia de actualizado.
○ FixedDataUpdateFormModel(): se encarga de obtener toda la información de una tarea en concreto, para que a través del controlador podamos ver el formulario con los datos cargados.
○ DeleteTasksModel(): haciendo uso de un identificador del registro, actúa sobre la base de datos ejecutando la operación de borrado.

<br>

<a name="backend"></a>

## Front-end

<br>

<a name="estructura-de-archivos"></a>

## Estructura de Archivos

Descripción de la estructura de archivos del proyecto.

```
M12_WebApp
│
├─ assets
│  └─ jefes_dptos_docs
│     ├─ JuanCarlos_GonzalezRuiz_foto.jpg
│     ├─ LauraMaria_MartinezPerez_foto.jpg
│     └─ LuisAlejandro_SanchezLopez_foto.jpg
│
├─ login
│  ├─ controller
│  │  └─ LoginController.php
│  ├─ model
│  │  └─ UserModel.php
│  ├─ view
│  │   └─ LoginView.php
│  ├─ login.php
│  ├─ logout.php
│
├─ secciones
│  ├─ employees
│  │  ├─ empleados_docs
│  │  ├─ controllers
│  │  │  └─ EmployeesController.php
│  │  ├─ model
│  │  │  └─ EmployeesModel.php
│  │  ├─ view
│  │  │  ├─ CreateEmployeesView.php
│  │  │  ├─ EditEmployeesView.php
│  │  │  └─ EmployeesView.php
│  │  ├─ create_employees.php
│  │  ├─ edit_employees.php
│  │  └─ index_employees.php
│  │
│  └─ tasks
│     ├─ controllers
│     │  └─ TasksController.php
│     ├─ model
│     │  └─ TasksModel.php
│     ├─ view
│     │   ├─ CreateTasksView.php
│     │   ├─ EditTasksView.php
│     │   └─ TasksView.php
│     ├─ create_tasks.php
│     ├─ edit_tasks.php
│     ├─ index_tasks.php
│
├─ templates
│   ├─ footer.php
│   └─ header.php
│
├─ bd.php
└─ index_main.php
```

<br>

<a name="capturas"></a>

## Capturas

<br>

<a name="demo"></a>

## Demo

<br>

<a name="licencia"></a>

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Para más detalles, consulta el archivo [LICENSE](LICENSE).

<br>

<a name="autor"></a>

## Autor

Este proyecto fue desarrollado por Juan Cumbe. Si tienes alguna pregunta o sugerencia sobre el proyecto, no dudes en contactarme a través de [e-mail](mailto:hello@juancumbe.com) o perfil en [Linkedin](https://www.linkedin.com/in/juancumbeq/). También puedes visitar mi sitio web [juancumbe.com](juancumbe.com). 😊
