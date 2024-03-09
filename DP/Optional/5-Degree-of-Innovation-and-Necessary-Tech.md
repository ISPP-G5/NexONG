# Grado de Innovación y Tecnología Necesaria - Devising a Project


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
2. Nuestro Grado De Innovación
3. Requisitos Tecnológicos Previos
4. Backend
5. Frontend
6. Otras tecnologías a utilizar


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
   <td>15/2/2024</td>
   <td>Primera versión</td>
  </tr>
  <tr>
   <td>2.0.0</td>
   <td>18/02/2024</td>
   <td>Segunda versión</td>
  </tr>
</table>



<br/>

# 

<br/>


# 1. Introducción

El propósito de este documento es describir el grado de la innovación tecnológica que propone nuestro proyecto _NexONG_ y las tecnologías necesarias para el desarrollo de este producto, así como el razonamiento que nos ha llevado a elegirlas.

La aplicación web tiene como objetivo gestionar cursos, eventos, donaciones y usuarios con diferentes roles de dos ONG y proporcionar una interfaz sencilla para la administración educativa, la gestión de voluntarios y la interacción con los familiares y socios. Deberemos, como equipo, alcanzar todos estos requisitos mientras que proveemos el mejor servicio posible a las entidades clientes, y sobre todo, que las ONG puedan hacer un buen uso de su portal web.


# 2. Nuestro Grado De Innovación

Entendemos la innovación como el proceso por el cual se transforma una idea en un producto o servicio que trae algo nuevo a un mercado,  o también a la incorporación de un novedoso proceso de fabricación o nuevos métodos de organización o de comercialización. En general, se habla de tres grados de innovación: incremental, radical y transformacional. 

La innovación incremental se refiere a pequeños cambios en un producto o proceso, también conocido como innovación continua. Luego, la innovación radical se refiere a cambios significativos a lo que ya existe. Finalmente, la innovación transformacional se refiere a cambios que transforman completamente lo que ya existe en algo distinto.

En el caso de nuestro proyecto, _NexONG_, trabajaremos para realizar una innovación sobre todo incremental, al proporcionar unos portales web más completos y fáciles de usar orientados a ONGs, si tenemos en cuenta que estas plataformas ya contaban con sus respectivas páginas web. 

Desde otro punto de vista, al crear estas aplicaciones web desde cero para así obtener un mejor producto, podríamos estar hablando de una innovación radical ya que cambiaremos virtualmente todos los aspectos del producto. Sin embargo, no podríamos referirnos a una innovación transformacional, ya que sigue siendo un portal web lo que desarrollaremos, y no otro tipo de producto nuevo o diferente.

Estas innovaciones sirven para mejorar la sociedad dentro de lo posible, con unas plataformas nuevas y accesibles para estas entidades sin ánimo de lucro. Tomamos la decisión de crear un producto desde cero al encontrarnos con tecnologías anticuadas existentes por parte del cliente, y tras llegar a un acuerdo mutuo con ellos, se acordó que sería la mejor forma de continuar con el proyecto.


# 3. Requisitos Tecnológicos Previos

El objetivo del proyecto _NexONG_ es proveer una herramienta que aporte la gestión de eventos y voluntarios a nuestros clientes, en este caso dos ONG, en las que el profesorado es constituido por un grupo de voluntarios y los beneficiarios pueden estar en distintos rangos de edad según la organización. La interfaz deberá ser sencilla y de uso fácil, siendo escalable y admitiendo unas 250 personas como mínimo al inicio.

Generalmente, las funciones a desarrollar consisten en: funcionalidades de administrador para la gestión de profesores-monitores, gestión de eventos y cursos, gestión de beneficiarios y gestión de voluntarios y socios, además de tener secciones de noticias y bandeja de entrada para el usuario.

Finalmente, es importante que la aplicación contenga una cláusula de privacidad y manipulación de datos según la legislación vigente.


# 4. Backend

Como ha sido mencionado previamente, este proyecto trata de una plataforma web de tamaño mediano diseñada para satisfacer las necesidades de una organización sin ánimo de lucro educativa que incluye administradores, educadores, familiares, voluntarios y socios.

Para crear la lógica empresarial y la gestión de los datos, es decir, el _Backend_, existen varias alternativas. Quitando las tecnologías con las que el equipo _Backend_ está menos familiarizado (como puede ser _Ruby on Rails_ o _Laravel_), destacan _Express.js,_ _Flask_, _Spring Boot_ y _Django_.

Entre los requisitos funcionales, no hay ninguno que sea particularmente complejo o requiera de una tecnología en concreto. Entre los requisitos no funcionales cabe destacar que la plataforma debe ser escalable, permitiendo desde un principio el uso simultáneo de 100 personas con un rendimiento aceptable y debe ser segura para proteger la información confidencial de los usuarios. En este caso, cualquiera de las tecnologías podría usarse también. 

_Express.js_ y _Flask_ son frameworks minimalistas, perfectos para aplicaciones rápidas de pequeño tamaño. Sin embargo, para implementar esta plataforma es mejor usar un framework que esté mejor estructurado y que ofrezca más funcionalidades sin instalar paquetes de terceros.

_Spring Boot_ es una tecnología perfectamente válida, con numerosos recursos y el equipo está bastante familiarizado con ella. Sin embargo, es una tecnología bastante antigua que requiere una configuración inicial muy compleja y requiere bastante recursos debido a que funciona mejor con aplicaciones de gran tamaño.

Luego, _Django_, por su parte, también es una tecnología válida con muchos recursos. La configuración inicial de _Django_ es mucho más sencilla y el flujo de trabajo sería más productivo para este alcance de proyecto. Cabe mencionar que el equipo de trabajo está familiarizado a esta herramienta, por la que finalmente, tras una votación, ha sido elegida para la estructura del Backend de _NexONG_.

Para el desarrollo de la base de datos, usaremos _SQLite_ por su simplicidad y ligereza. Es también fácil de implementar con _Django_. Después, en el entorno de producción podremos cambiar sin problema a una base de datos que ofrece mayor escalabilidad y rendimiento como _MySQL_ o _PostgreSQL_.


# 5. Frontend

En cuanto al Frontend, hay que tener en cuenta que la plataforma debe ofrecer una interfaz sencilla y moderna. Para ello se puede usar cualquier tecnología moderna compatible con _Django_. Hay varias alternativas, entre las que destacan las plantillas de _Django_ (DTL),  simple _Javascript_ o algún framework independiente como pueden ser _React_, _Vue.js_ o _Angular_.

Las DTL se integran perfectamente con _Django_ y ofrecen un muy buen rendimiento, pero no ofrecen poca interactividad y escalan mal, por lo que para el alcance y los requisitos de este proyecto no vienen bien. 

Usar _Javascript_ puede ser tan potente como usar un framework si se usa bien,  ya que puede llegar a ofrecer más rendimiento y mucha flexibilidad, sin embargo, el flujo de trabajo sería poco eficiente y la estructuración del código podría ser pobre. 
Por esta razón usaremos un framework para el Frontend.

Entre cuál framework es mejor usar, la única diferencia es la preferencia personal, puesto que con cada framework se podrían implementar los requisitos perfectamente. 

Tras una votación grupal, hemos decidido que usaremos _React_ debido a que se integra fácilmente con _Django_,  cuenta con un robusto ecosistema lleno de recursos y que gran parte del equipo Frontend está familiarizado con ella. 
Otra ventaja de usar _React_ es el hecho que la herramienta que utilizamos para los mock-up del diseño _Frontend_, [Figma](https://www.figma.com/proto/uCBbvfz4BH6ooGEeeFRyZO/ISPP?type=design&node-id=12-92&t=GRmI9oACDddGzOnO-1&scaling=scale-down&starting-point-node-id=12%3A92&show-proto-sidebar=1&mode=design), permite importar y trabajar con ella. 
El uso de _React_ permitirá estructurar el proyecto mediante el uso de componentes y facilitará la creación de interfaces de usuario altamente interactivas y dinámicas, como bien quiere nuestro cliente.


# 6. Otras tecnologías a utilizar

Dado el nivel acordado para el proyecto, se puede afirmar que también haremos uso de _Github_ como herramienta de control de versiones del código fuente, además de hacer uso de su tabla ‘Kanban’ para permitir a los miembros del grupo asignarse las tareas necesarias. 
La gran ventaja que proporciona esta plataforma es la facilidad de acceso para todos los participantes y el sistema de ‘ramas’ y ‘commits’ para controlar el versionado del proyecto. 
Además, poniendo en práctica técnicas de trabajo como _git flow_ podremos aumentar la calidad de nuestro código y facilitar la aportación de cada miembro.

La creación tanto de los documentos como las presentaciones se realizará mediante _Google Docs_ y _Google Slides_, y serán organizados en _Google Drive_, en la nube. 
Esta decisión fue tomada ya que es muy fácil y gratuito compartir y editar documentos simultáneamente entre varias personas.


La mensajería entre los integrantes del grupo y las reuniones virtuales tendrán lugar en _Discord_, al proporcionar un sistema más organizado con canales de chat y voz para categorías en concreto. 
Aún así, para el envío de mensajes con carácter más informal y que no tengan impacto sobre el proyecto,  también utilizamos _Whatsapp_, siempre tratando de hacer uso de _Discord_ para tratar temas relevantes.

La Inteligencia Artificial también es una herramienta útil para programar o para hacer consultas para la documentación del proyecto, cuyos ‘prompts’ estarán recogidos en el documento ’Uso de la IA’. 
Las tecnologías que utilizaremos puntualmente son _Chat GPT_, _Bard_ y el _Copilot_ de _Github_.
