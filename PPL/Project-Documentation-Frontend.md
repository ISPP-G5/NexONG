# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp; 5-Project-Documentation-Frontend
# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp; NexOng - Grupo 5

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

<a name="br2"></a> 

## Índice
1. Registro de cambios
2. Introducción
3. Trabajo realizado
4. Trabajo futuro
5. Trabajo por mejorar

## Registro de cambios
**Versión** | **Fecha** | **Descripción**| **Redacción** | **Revisión**
--- | --- | --- | --- | --- 
1.0.0 | 29/4/2024 | Semana 12 |CLAUDIA GILABERT PRIETO| AURORA NAVAS JIMÉNEZ


## Introducción
El objetivo principal de este documento es la creación de una guía que contenga información sobre las tareas que se han realizado durante el desarrollo del proyecto, que tareas han quedado pendiente y que se podrían implementar en el futuro así como que partes de las ya implementadas podrían ser mejoradas para así hacerlas más eficientes y ajustarnos de mejor manera a los requisitos dados por la ONG Manos Abiertas con Norte, nuestro actual cliente.

Importante mantener en mente que en este documento solo se esta teniendo en cuenta la parte correspondiente al Frontend. Se ha decidido hacer en dos documentos separados para facilitar la lectura y entendimiento.
## Organización del repositorio
En el caso de nuestro grupo nexONG se acordó la creación de una organización en la que se crearían diferentes repositorios: uno para la documentación, otro para la landing page, otro para el Backend y finalmente uno para el Frontend.

Al tener diferentes repositorios de trabajo, a nosotros personalmente nos facilitó el trabajo ya que nos permite localizar la información que queremos de manera rápida, en cambio si todo estuviera en un mismo repositorio sería mas complicado. 

En el repositorio del Frontend se ha seguido el flujo de trabajo de GitFlow dónde la rama Develop es en la que se ha ido desarrollando, se ha creado una rama Deploy para el despliegue que sigiendo la estructura de GitFlow es la rama de publicación. Además, el contenido de Develop se pasa a Main para realizar un release con su correspondiente etiqueta.

A la hora del desarrollo se utilizó el apartado de issues para describir que tareas hay que realizar si son features o fixes (estas son las dos principales que hemos tenido) así como los issues relacionados con el release y despliegue. Se han utilizado plantillas para los issues para facilitar que todos tengan la misma estructura, aunque si hiciera falta se puede publicar sin usar las plantillas.

Cada issue estaba asiganado a una o dos personas como mucho con su etiqueta correspondiente, deadline y proyecto. Cada issue completado es seguido por su correspondiente pull request donde tenemos un workflow de Codacy para asegurar que se cumple la calidad del código. Cada pull request es revisada por tres personas, siendo siempre una de ellas la Team Leader del Frontend para garantizar que el trabajo realizado cumple con lo esperado. 

La Team Leader, era también la que creaba y asignaba los issues a cada persona de su grupo. Esta organización, creación y asignación de tareas era consultada entre PM y el team leader del backend para que se supiera en todo momento en que se iba a trabajar y si lo que se quería realizar por parte del Frontend es posible (teniendo en cuenta que la parte correspondiente del Backend estuviera creada). 

Como se ha indicado se han utilizado los proyectos de GitHub ya que facilita la organización de los repositorios y sus tareas gracias al tablero Kanban que ofrece que permite visualizar la tarea,  el/la asignado/a, el deadline y los revisores. Los revisores también eran establecidos por los Teams Leader en su correspondiente repositorio para así garantizar que todos los miembros revisaran código de sus compañeros.

## Trabajo realizado
Una vez recopilados los requisitos de parte de nuestro cliente, se analizaron y estudiaron para poder así entender de manera más profunda que es lo que necesitaban y esperaban del software que se iba a desarrollar. 

Una vez con toda esa información en mente, se crearon los mock-ups de la aplicación. Se pensó en todo momento tener una interfaz sencilla para facilitar a futuros usuarios el uso de nuestro software. 

Con toda la información precedente de los requisitos así como el diseño de la aplicación, se realizó una primera planificación de las tareas a realizar que por cuestiones del tiempo disponible así como organización del equipo se vió la necesidad de reducir el alcance y de realizar una re-planificación.

A continuación se explicará de manera más detallada que se ha ido realizando y para ello se va a dividir en 5 secciones, una por rol (administrador, socio, educador, voluntario y familias ) y dentro de cada uno de estas divisiones se proporcionará información de lo que cada rol puede realizar.

El acceso a la información procedente del backend por parte del Frontend se realizó mediante consultas a la API Rest desarrollada desde el Backend usando Django Rest. Para poder hacer estas solicitudes se ha utilizado la librería axios.
Se ha utilizado para la calidad del código Codacy y evitar sobre todo duplicaciones de código para forzar el hecho de trabajar en componentes y sacarle el máximo partido a React.

#### Rol de administrador
El rol de administrador es uno de los más importantes para la ONG, ya que le permitiría realizar diferentes acciones como la gestión de voluntarios de manera digitalizada. Actualmente, toda gestión realizada por la ONG se basa en creación de Excels lo que hace todo un poco complicado, en palabras de la coordinadora de la ONG.
Todo lo que viene a continuación es desde la perspectiva de un usuario que ha inciado sesión como administrador.
##### Voluntarios
Las tareas realizadas en este apartado estan relacionadas con el proceso de gestión de voluntarios:

- Listado de voluntarios: el usuario que acceda con el rol de administrador va a poder visualizar los voluntarios registrados en la ONG.

- Proceso de aceptación de un voluntario: una vez que los voluntarios han realizado todos los papeles necesarios para presentar su solicitud, deben esperar a que la ONG los acepte o los rechaze. El administrador tiene accesso a la información del voluntario que ha realizado la solicitud: puede descargarse en formarto ZIP todos los archivos correspondiente a esa solicitud, así como poder aceptar o rechazar.

- Editar/Borrar voluntario: además de esas dos acciones anteriores, se añadió por solicitud de la ONG la opción de que el administrador pueda editar los datos del voluntario así como darlo de baja si se deseara.
  

##### Familias
Las pantallas correspondiente a familias desde la perspectiva de administrador tiene una estructura muy similar a la de voluntarios ya que al igual que en la parte explicada con anterioridad se puede visualizar un listado de las familias registradas en la plataforma con la información correspondiente de sus hijos. Además, presentan también un sistema de gestión de solicitudes. Estas son creadas y mandadas por las familias y contienen la información correspondiente a sus hijos, ya que al final son ellos los que hacen uso de los servicios de la ONG.

##### Educadores
El trabajo realizado en educadores se basa en dos principales partes:

- Listado de educadores: se va a poder visualizar un listado de los educadores registrados con la ONG. Además, el administrador va a poder editar sus datos así como borrar su perfil si lo deseara.
- Registro de nuevos educadores: mediante las reuniones con la ONG, descubrimos  que el rol de educador es el único que no se registra el mismo en la ONG, todos ese papeleo es llevado a cabo por la ONG. Por ellos en la pestaña de educadores aperece una sección para poder proceder con este paso.Los educadores son informados por parte de la ONG de los datos de su cuenta para poder así iniciar sesión a las pantallas correspondiente de ese rol espcifíco.

##### Socios
Al igual que en todos los roles anteriores, aparece el listado de socios así como la posibilidad de editar y borrar la cuenta del socio, si el administrador deseará. Aparte de esta funcionalidad, aquí se pueden encontrar dos no vistas de manera anterior:

- Creación de reuniones: una de las acciones que una persona que sea socia de la organización puede hacer, es ir a las reuniones que se van a realizar. Por ello el administrador va a poder crear estas reuniones que una vez que se hayan creados, el socio podrá ver cuando tienen lugar desde su perfil.
- Exportación de donaciones: los administradores pueden exportar un documento en formato Excel,PDF o CSV con la siguiente información sobre las doncaciones realizdas por los socios:cantidad, frecuencia, titular y fecha.

##### Clases
En esta sección podemos encontrar varias funciones diversas:
- Listado de clases: si existen clases, aparecerá un listado con información de las diferentes clases que existen. 
- Creación de clases: los administradores son los responsable de la creación de las clases y por tanto deben de poder crearlas.
- Crear Horario: cada clase creada tiene un horario especifico, en la opción de crear horario lo que se permite es que con una clase creada se pueda crear el horaro de las diferentes clases.
- Ver horarios: nos permite visualizar lo que se ha creado anteriormente.
##### Eventos
En la sección eventos se muestra un calendario en el cual se va a mostrar:
- Creación de eventos: se van a poder crear dos tipos. Actividades que corresponden a una clase especifica (se podría también llamar excursiones) y eventos accesibles para todos los que pertenecen a la ONG.
- Visualización calendario: en el calendario se van a poder observar los eventos, las actividades, las reuniones.
##### Sugerencias 
Los usuarios pueden realizar sugerencias a la ONG y esta las puede leer y una vez leídas borrarlas.
##### Documentos
En la parte de la pantalla principal accesible a todo el mundo (no hace falta tener una cuenta), encontramos el apartado de transparencia (se explicará en breves de manera más profuprofunda) que cada año debe ser actuaizado con nuevos documentos y para facilitar esto y que se puede hacer de manera automática se ha creado un formulario con este objetivo. El formulario consiste de los siguiente campos (son los que se necesitan de cada documento): título, tipo de documento en un desplegable, adjuntar documento y le fecha.

Por último, el administrador puede actualizar los datos de su perfil si lo deseará. Esta acción es posible en cada uno de los roles por tanto no se va a volver a indicar para que el documento no sea repetitivo.

#### Rol de Educador 
Este rol puede realizar las siguientes acciones:
##### Evaluación Diaria 
La organización nos transmitió que una de las partes mas importantes para ellos era lo relacionado con la evaluación y que presentan diferentes tipos de evaluaciones entre ellas la diaria. Un educador va a poder filtrar por sus clases y solo los alumnos de ellos van a aparecer y poder ser evaluados indicando una puntuación (que depende del tipo de evaluación creado), un comentario y la fecha. Además, si desean ponerse en contacto con la familia tienen acceso a esa información. 
##### Evaluación Anual
La evaluación anual es igual que la anterior pero se realiza de año en año.
Ambos tipos de evaluaciones pueden ser mejorados en el futuro y se proporcionará más información.
##### Actividades
En este apartado se muestran las actividades creadas por el administrador que pertenezca al educador y sus alumnos, mostrando información si tienen la autorización por parte de sus padres o tutores legales a participar en ella o no. 
#### Rol de Socio
El socio va a tener un calendario donde se va a mostrar las futuras reuniones a las que puede ir si lo desea. Además, el perfil del socio es algo diferente ya que presenta un apartado de renovar o cambiar cuota de la donación. Esto se realiza mediante un formulario en cual hay que indicar el titular de la cuenta bancaria, el IBAN, cantidad a donar y frecuencia mediante el uso de checkbox. 

Si el socio deseara cancelar su suscripción como socio, con pulsar el botón borrar cuenta sería suficiente. 
#### Rol de Familia
El rol de Familia es otro de los más importantes a destacar, ya que las familias son los principales en hacer uso de los servicio que la ONG ofrece. 

- Niños: en esta pestaña van a poder visualizar los datos de su hijo así como registrar nuevos hijos si lo desean. Una vez realizada la solicitud este deberá ser aceptada por el administrador.
- Evaluación diaria: las evaluaciones dadas por los educadores, van a ser visualizadas por la familia indicando en grande la puntuación, el nombre de la evaluación, el nombre del alumno, la clase y la fecha.
- Evaluación anual: es igual que el caso previo pero en este caso se visualizarían las evaluaciones de año en año.

- Autorizaciones: se diferencian dos diferentes apartados. Autorizaciones hechas que muestran la información relacionada con una actividad en la que ya se ha completado y en eventos disponible muestran eventos que van a llevarse a cabo y necesitan que se complete todavía la autorización.
-Calendario: en el calendario se va a mostrar las clases de los hijos de la familia, las excursiones y los eventos. Cada uno con un color diferentes para hacer lo más visual y claro. Si se presiona sobre uno de ellos más información se muestra

#### Pantalla principal 
La pantalla principal hace referencia a toda aquella parte de la aplicación a la que se puede acceder sin tener una cuenta. Se podría pensar que no es tan importante ya que no se realiza ninguna funcionalidad de gestión en el tema de la ONG pero es igual de importante o incluso más ya que muchos de los apartados introducidos son necesarios para que la organización reciba subvenciones.
La información incluida ha sido proporcionada por la propia organización u obtenida de su página web actual.

Otra información importante, es que se ha seguido la misma estrctura en todas las diferentes pestañas dentro de lo posible para mantener una interfaz limpia.
###### Pantalla Home
Se hace una breve descripción de la organización así como mostrar diferentes apartados a los que pueden ser redirigidos si se quisiera mayor información.


###### Asociación
- Nosotros: breve presentación de Manos Abiertas con Norte, indicando donde se centra su trabajo así como que trabajo llevan acabo. Además de un vídeo que realizaron en el año 2020/2021 preguntando a alumnos sobre que es para ellos Manos Abiertas.
- Historia: se habla sobre cuando se creó y como comenzó la aventura de esta organización y como ha ido creciendo con el paso del tiempo.
- Misión, visión y valores: como se puede deducir por el titulo otorga información sobre esos tres pilares esenciales para cualquier organización sin ánimo de lucro.
- La Salle: al partener a la red de colegios La Salle, era un requisito esencial de Manos Abiertas, incluir información sobre que es lo que realiza La Salle en el área de colaboración con asociaciones.
- Organización: explica como se dividen y quién ocupa cada puesto. Este es un punto de mejora para el futuro.
- Transparencia: anteriormente en la parte de administrador se comentó sobre un apartado de documentos. Los documentos que se introduzcan aparecerán en la tabla de esta pestaña.
- Entidades Colaboradoras: esencial también indicar que tienen asociado que dan ayuda y subvenciones. Se muestran con una imágen así como un enlace hacia su página web.

###### Actividades
- Actividades: breve resumen de las actividades proporcionadas por la ONG.
- Aula abierta: una de las actividades que se ofrece que consiste en apoyo educativo. Aquí se explica de que trata esta.
- Aula de convivencia: proporciona ayuda educativa a menores con conducta disruptivas. Se explica que es lo que se realiza con este programa. 
- Talleres familiares: la asociación quiere mostrar y dar apoyo a las familias y para ello crearon esta actividades. Se muestra explicado que es lo que se realiza. 
- Club de verano: actividad que se realiza en verano donde se realizan talleres, excursiones,...
- Campamento de verano: cada año se realiza esta actividad con la Asociación Rutas Sevilla.

En el apartado de actividades se proporciona información sobre que servicios ofrecen y que es lo que se hace para atraer a personas que puedan necesitar de estos servicios

##### Agenda 2030
Toda organización que incluya en su página web información relacionada con la Agenda de sostenibilidad de 2030 reciben más subvenciones. Por ellos la necesidad de incluirla. Además, indicando como intenta aplicar sus puntos a través de la organización.

###### Donaciones
Si está interesado en realizar una donación a la ONG, es posible. Si quiere solo hacer esa acción una vez, haz una donación puntual en la que debe indicar su nombre, apellidos, correo electrónico y el método de pago: tarjeta de credito o tranferencia y bizum.
Si esta interesado en donar de manera recurrente podra pulsar en el botón de registrase y ser redirigido a esa pestaña.

###### Voluntarios
¿Qué es una organización sin ánimo de lucro sin la ayuda de voluntarios?. Los voluntarios son una parte esencial de cualquier asociación y en este apartado se quería proporcionar información sobre ello así como el botón para ser redirigido hacia el registro de voluntario.

###### Sugerencias
Actualmente, Manos Abiertas acepta sugerencias de manera presencial en un buzón que tienen pero estaban interesado en digitarizarlo. Para ello se ha creado la pantalla sugerencias donde cualquier persona puede dejar un comentario si lo desea.

##### Registro 
Como indicado de manera anterior existen 5 roles. De esos 5 solo puedes registrarte en tres: socios,voluntarios y familias ya que los educadores son registrados por el administrador y no se debe dar una opción de registrarse como adminsitrador a cualquiera ya que contiene mayor poder de realizar acciones.

En este apartado completas tus datos correspondientes, aceptas la política de privaciad y seleccionas el rol en el que estas interesado. 

Una vez completado esto y dependiendo del rol eres redirigido a un segundo formulario para intorducir los datos necesarios y específicos  de cada uno de esos roles. 

El usuario que se registre, para poder usar su cuenta para iniciar sesión debe verificar su correo electrónico. 

###### Inicio de sesión
Una vez verificado el correo y completados los formularios serás redirigido a la pantalla correspondiente a tu rol. 

Además de todo lo explicado anteriormente de tareas realizadas, se han añadido mensajes de error y éxito en cada consulta para transmitir al usuario si la acción que realiza es correcta o no. Para estos mensaje hemos usado la librería Toastify disponible para React.
###### Cabecera y Pie
Se ha creado una cabecera con el logo de la ONG que si se presiona te redirige a la página principal y se han añaido los diferentes enlaces de todas las páginas explicadas anteriormente.

En el pie se ha indicado el correo electrónico de la asociación, los teléfonos, el número del Fax y el CIF. Además de la direción de ellos así como sus redes sociales.

También hemos implementado mensajes de confirmación antes de acciones de borrar para comprobar que el usuario es consciente de la acción que va a realizar y las consecuencias que eso lleva. 

## Trabajo pendiente por realizar
Este apartado es necesario ya que debido a los limites de tiempo y que Manos abiertas en cada reunión iba añadiendo más requisitos y funcionalidades que se podrían incluir.Con todo est en mente, se decidió reducir el alcance haciendo imposible la implementación de todo pero no queremos que se quede en el olvidó y por ese mismo motivo queremos incuirlo en este documento: 

- La ONG solicito que a la hora que un voluntario se registre, se considere introducir un nuevo campo al formulario: descripción dónde introduzcan información sobre ellos. Este campo luego podrá ser editado en el caso de que su solicitud sea aprobada.

- En el mismo ángulo, los educadores deberían también tener un campo de descripción para proporcionar información sobre ellos. Esto se podría añadir como un nuevo campo que aparezca en el perfil. Además, debería ser editable.

- Actualmente, solo se ha incluido un desplegable para exportar datos en la parte de socios. Por parte del backend se han creado funciones para exportar la información de cada uno de los roles pero desde el frontend no se ha podido realizar ya que no era una funcionalidad principal.

- Tuvimos que cancelar la parte de proyectos. Este apartado se decidió alcanzar debido a una gran cantidad de dudas de como sería más útil hacia la asociación ya que ni ellos lo tienen muy claro. La idea es que los proyectos puedan ser creados por los administradores. Además, los educadores tendrían la posibilidad de evaluar estos proyectos de manera diaria y anual.
- Otro de los aspectos que no se realizó es la parte de los centros educativos. Es cierto que es una funcionalidad bastante interesante y útil ya que facilitaría el contacto entre los colegios y la asociación para aquellos alumnos que por conducta disruptiva han sido expulsados de sus colegios y van a la organización para tener apoyo educativo. La razón principal para no realizarlo fue que estamos muy limitados por el tiempo y no se estaba cien por cien seguro de si sería usado por lo centros educativos y por ello se dejo en un segundo plano.

- Actualmente, existe un log in social que funciona tanto por parte del backend así como el frontend pero no se muestra en la aplicación porque faltaba por crear los cuestionarios correspondiente de registro para un usaurio que utilize este método de incio de sesión. Al enterarnos de que la funcionalidad probablemente no fuera muy utilizada por los futuros clientes, no se le dió prioridad y nos centramos en otras partes que se consideraban de mayor importancia.

- Para el futuro, nos encantaría poder digitalizar los métodos de contactos. Por ejemplo educadores pueden actualmente ver la información ed la familia del estudiante, lo ideal es que el educador pudiera usar directamente la platarforma para esa comunicación.  Al igual nos gustaría incluir esta opción desde la perspectiva de la familia si se quiere poner en contacto con el educador de su hijo.

- Añadir un dialogo en las pantalla de evaluación de la evaluación con la información del educador de su hijo (igual que esta hecho en educadores que ve las familias pero a la inversa, las familias ven los datos de los educadores)

- En las pantallas relacionadas con la pantalla principal, las actividades de su página web actual incluye más opciones. En un futuro estaría bien volver a preguntar a la ONG sobre ello por si se quisiera incluir.


## Cosas para mejorar
Somos autocríticos de nuestro propio trabajo sabiendo y siendo conscientes de que siempre habrá cosas que se pueda mejorar para hacer las más accesibles. No solo se tiene esta autoevaluación en cuenta para el apartado en el cual estamos si no también el feedback recogido sobre las pruebas de los usuarios piloto. En general, la mayoría de ellos se tuvieron en cuenta y se corrigieron de manera inmediata ya que era errores considerables como no mostrar mensajes de error. Aunque cabe destacar que el feedback dado como sugerencia no se consideró  debido al tiempo y se decidió trabajar sobre aquello más relevantes y que no funcionaba como se esperaba. A continuación se va a mostrar aspesctos abiertos a mejoras del software que actualmente tenemos desarrollado.

- En el primer feedback recibido, se proporciono la sugerencia de que en las pantalla (iniciando sesión como administrador) de socios y educadores la creación de asambleas y el añadir educadores de manera respectiva podrían cambiarse a un botón en vez de tener que cambiar de pestaña. Este feedback se ha tenido en cuenta y por eso se indica en este apartado de mejoras.
- Por otro lado nos gustaría comprobar que la interfaz que ha sido creada es las más adecuada para nuestro usuarios potenciales comprobando que nuestra user experience es satisfactoria o no.

- Estando en la pantallas correspondientes al rol de administrador se querría añadir mayor información sobre la pestaña del rol que se esta visualizando. Ahora mismo incluye los datos básicos como pueden ser nombre y apellido. 
El administrador debería de poder acceder a otros datos como la documentación de los voluntarios registrados, acceder a los documentos de las familias, y la tarjeta sanitaria.
También podría quere acceder a los socios y poder ver de manera clara la cantidad que dona y cada cuanto tiempo.En la información de educadores no estaría que se mostrará el correo electrónico si el administrador quisiera contactar con el.

- El tema de las evaluaciones podría ser mejorada de manera considerada en el futuro. Desde el backend existe la opción de crear tipos de evaluaciones, cosa que actualmente no se considera desde el frontend. Además, se podría lograr ver evaluaciones pasadas por parte del educador si quisiera. Además, de añadir evaluaciones trimestrales que no esta actualmente contempladas desde el frontend.

## Conclusión
Se ha desarrollado una pequeña guía con la información correspondiente a que se ha realizado durante el proyecto, que se puede mejorar de ellos y que a quedado por implementar. Aunque parezcan muchas cosas dejadas en el tintero ya sea por mejoras o para el futuro, estamos todo el grupo, especialmente el equipo del frontend del trabajo logrado y conseguido durante la etapa de desarrollo. Para muchos, el uso de React ha sido algo nuevo o si no lo ha sido que han tenido que recordar como funcionaba.

























