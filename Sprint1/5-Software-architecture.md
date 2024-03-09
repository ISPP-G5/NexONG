# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Arquitectura - Sprint 1


***MIEMBROS***:

<table>
  <tr>
    <td>AURORA NAVAS JIMÉNEZ</td>
    <td>MARÍA NÚÑEZ REYES</td>
    <td>CLAUDIA GILABERT PRIETO</td>
  </tr>
  <tr>
    <td>MARTA INÉS GONZÁLEZ DIÁNEZ</td>
    <td>FÉLIX ÁNGEL GUDIEL GÜEMES</td>
    <td>MIGUEL ANGEL ROMALDE DORADO</td>
  </tr>
  <tr>
    <td>FRANCISCO DE ASÍS ROSSO RAMÍREZ</td>
    <td>PABLO PERIÁÑEZ CABRERO</td>
    <td>FRANCISCO JAVIER CALDERÓN RODRÍGUEZ</td>
  </tr>
  <tr>
    <td>PEDRO LOPEZ RUZ</td>
    <td>IVÁN RAMÍREZ LARA</td>
    <td>SAMUEL LUIS RODRÍGUEZ MANESS</td>
  </tr>
  <tr>
    <td>MANUEL ORTIZ BLANCO</td>
    <td>SERGIO AGUAYO OROZCO</td>
    <td>JUAN LUIS RUANO MURIEDAS</td>
  </tr>
  <tr>
    <td>MANUEL FRANCISCO BARCIA JIMENEZ</td>
    <td></td>
    <td></td>
  </tr>
</table>


## Índice

1. Introducción
2. Contexto de la arquitectura
3. Diseño de la arquitectura
4. Comunicación entre cliente y servidor
5. Conclusiones


## Registro de cambios


<table>
  <tr>
   <td><strong>Versión</strong>
   </td>
   <td><strong>Fecha</strong>
   </td>
   <td><strong>Descripción</strong>
   </td>
  </tr>
  <tr>
   <td>1.0.0</td>
   <td>22/2/2024</td>
   <td>Primera versión</td>
  </tr>
</table>



<br/>

# 

<br/>


# 1. Introducción

Este documento tiene como objetivo justificar la elección de la arquitectura cliente-servidor para el desarrollo del sistema de gestión de una Organización No Gubernamental (ONG). La adopción de esta arquitectura proporciona una estructura sólida y eficiente para el diseño, implementación y mantenimiento de un sistema que cumpla con los requisitos funcionales y no funcionales definidos por la organización.

La ONG enfrenta desafíos significativos en la gestión de sus actividades, recursos y relaciones con donantes y beneficiarios. Para abordar estos desafíos de manera efectiva, se requiere un sistema de información robusto y escalable que permita la gestión eficiente de datos y procesos críticos.

En este contexto, se ha evaluado una variedad de opciones arquitectónicas, y se ha determinado que la arquitectura cliente-servidor es la más adecuada para satisfacer las necesidades y objetivos del proyecto. Esta arquitectura proporciona una clara separación de responsabilidades entre el cliente, que se encarga de la interfaz de usuario y la presentación de datos, y el servidor, que gestiona la lógica de negocio y el almacenamiento de datos.

El documento proporcionará una descripción detallada de los componentes del sistema, la comunicación entre el cliente y el servidor, así como las razones fundamentales que respaldan la elección de la arquitectura cliente-servidor para este proyecto.


# 2. Contexto de la arquitectura

La elección de la arquitectura cliente-servidor para el sistema de gestión de la ONG se fundamenta en una serie de consideraciones que tienen en cuenta tanto las necesidades específicas de la organización como las tendencias y mejores prácticas en el desarrollo de software.

1. **Requisitos Organizacionales:**

   La ONG requiere un sistema de gestión que permita centralizar y organizar eficientemente la información relacionada con sus actividades, proyectos, donantes, voluntarios y beneficiarios.

   Se busca una solución que sea fácil de usar y mantener, permitiendo a los usuarios acceder a la información de forma rápida y segura desde diferentes ubicaciones y dispositivos.

   Es necesario garantizar la integridad y confidencialidad de los datos, así como la disponibilidad del sistema en todo momento para garantizar la continuidad de las operaciones de la organización.

2. **Tendencias Tecnológicas:**

   La arquitectura cliente-servidor es ampliamente reconocida como un enfoque eficaz para el desarrollo de aplicaciones web modernas, ya que permite una clara separación de responsabilidades entre la interfaz de usuario y la lógica de negocio.

   La adopción de tecnologías como Django para el backend y React para el frontend proporciona un conjunto de herramientas robustas y bien establecidas que facilitan el desarrollo ágil y la implementación de características avanzadas.

3. **Escalabilidad y Mantenimiento:**

   La arquitectura cliente-servidor ofrece la flexibilidad necesaria para escalar el sistema de manera modular, permitiendo agregar nuevas funcionalidades o modificar las existentes sin afectar otras partes del sistema.

   La separación de la lógica de negocio del frontend facilita el mantenimiento y la evolución del sistema a largo plazo, ya que los cambios en la interfaz de usuario pueden realizarse sin necesidad de modificar el backend.

   En resumen, la arquitectura cliente-servidor se presenta como la opción más adecuada para satisfacer las necesidades de la ONG en términos de eficiencia, seguridad, escalabilidad y mantenimiento. Proporciona una base sólida para el desarrollo de un sistema de gestión que contribuirá al éxito continuo de la organización en la consecución de sus objetivos.




# 3. Diseño de la arquitectura

El diseño de la arquitectura para el sistema de gestión de la ONG se basa en la arquitectura cliente-servidor, que proporciona una estructura clara y modular para el desarrollo de la aplicación. Este enfoque separa la interfaz de usuario (cliente) de la lógica de negocio y el almacenamiento de datos (servidor), lo que facilita la escalabilidad, el mantenimiento y la evolución del sistema.

1. **Cliente (Frontend):**

   El cliente se desarrollará utilizando React, un framework de JavaScript ampliamente utilizado para la construcción de interfaces de usuario interactivas y dinámicas.

   React permite la creación de componentes reutilizables, lo que facilita el desarrollo y la mantenibilidad del frontend.

   La interfaz de usuario se diseñará de manera intuitiva y amigable para el usuario, centrándose en la usabilidad y la accesibilidad.

2. **Servidor (Backend):**

   El servidor estará basado en Django, un framework de desarrollo web de alto nivel que fomenta el desarrollo rápido y limpio.

   Django proporciona un conjunto completo de herramientas para la gestión de la lógica de negocio, la autenticación de usuarios, el manejo de sesiones, la gestión de la base de datos, entre otros.



# 4. Comunicación entre cliente y servidor

La comunicación entre el cliente (frontend) y el servidor (backend) es fundamental para el funcionamiento del sistema de gestión de la ONG. Se utilizará una arquitectura basada en APIs RESTful para establecer una comunicación eficiente y estructurada entre ambas partes del sistema. A continuación, se detallan los aspectos relevantes de esta comunicación:

- **API RESTful:**

  Se implementará una API RESTful en el servidor utilizando Django REST Framework. Este marco proporciona herramientas poderosas para la creación de APIs web basadas en REST, incluyendo la serialización de datos, la gestión de peticiones HTTP y la autenticación de usuarios.

  La API estará compuesta por endpoints que representan recursos específicos del sistema, como usuarios, donaciones, proyectos, etc. Cada endpoint admitirá operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre estos recursos.

- **Formato de Datos:**

  Los datos intercambiados entre el cliente y el servidor se transmitirán en formato JSON (JavaScript Object Notation), que es un formato ligero y fácil de parsear que se adapta bien a las necesidades de una API RESTful.

  La serialización y deserialización de datos se gestionará de manera transparente mediante las capacidades integradas de Django REST Framework, lo que facilita la interoperabilidad entre el cliente y el servidor.

- **Métodos HTTP:**

  Se utilizarán los métodos estándar de HTTP (GET, POST, PUT, DELETE) para realizar operaciones sobre los recursos de la API.

  Por ejemplo, para recuperar datos de un recurso, se utilizará el método GET; para crear un nuevo recurso, se utilizará el método POST; para actualizar un recurso existente, se utilizará el método PUT o PATCH; y para eliminar un recurso, se utilizará el método DELETE.

- **Autenticación y Autorización:**

  Se implementarán mecanismos de autenticación y autorización en la API para garantizar que solo los usuarios autorizados puedan acceder a determinados recursos y realizar ciertas acciones.

- **Gestión de Errores:**

  Se establecerán códigos de estado HTTP apropiados para indicar el resultado de las operaciones realizadas en la API, como el éxito, la creación exitosa de un recurso, la actualización exitosa de un recurso, etc.

  Se proporcionarán mensajes de error detallados en caso de que ocurra un error durante el procesamiento de una solicitud, lo que facilitará la depuración y solución de problemas por parte de los desarrolladores del cliente.

  La comunicación entre el cliente y el servidor a través de una API RESTful proporciona una interfaz clara y flexible para la interacción entre ambas partes del sistema, lo que facilita el desarrollo, la integración y el mantenimiento del sistema de gestión de la ONG.



# 5. Conclusiones

La implementación de la arquitectura cliente-servidor con Django en el backend y React en el frontend ha resultado en un sistema de gestión eficiente y adaptable para la ONG. Esta estructura modular permite un desarrollo ágil, una interfaz de usuario intuitiva y medidas sólidas de seguridad. La separación de responsabilidades facilita el mantenimiento a largo plazo y la evolución continua del sistema. En resumen, la elección de esta arquitectura ha sido acertada para cumplir con los requisitos de la organización de manera efectiva.



