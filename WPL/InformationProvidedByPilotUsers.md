# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Feedback de los usuarios pilotos - WPL
# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;NexOng - Grupo 5

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
2. Sprint 2
	1. Feedback del grupo 11
	2. Feedback de Manos Abiertas con Norte
	3. Futuros cambios
3. Sprint 3
	1. Feedback del grupo 11
	2. Feedback de Manos Abiertas con Norte
	3. Futuros cambios


## Registro de cambios

| Versión | Fecha | Descripción | Redacción | Revisión
|---------|-------|-------------|---------------|---------------|
|1.0.0|28/03/2024|Feedback del Sprint 2|AURORA NAVAS JIMÉNEZ y MARÍA NÚÑEZ REYES | FRANCISCO JAVIER CALDERÓN RODRÍGUEZ|
|1.0.1|30/03/2024|Cambio de portada según failure conditions|AURORA NAVAS JIMÉNEZ |MANUEL ORTIZ BLANCO y PEDRO LÓPEZ RUZ|
|2.0.0|05/04/2024|Feedback del Sprint 2 de Manos Abiertas|AURORA NAVAS JIMÉNEZ |CLAUDIA GILABERT PRIETO|
|3.0.0|18/04/2024|Feedback del grupo 11 del Sprint 3|AURORA NAVAS JIMÉNEZ |CLAUDIA GILABERT PRIETO|

## 1. Introducción
El presente documento tiene como objetivo principal recopilar y analizar el valioso feedback proporcionado por los usuarios pilotos, previamente definidos en el documento **pilots.md**. Este proceso de retroalimentación juega un papel fundamental en el desarrollo y mejora continua de nuestra aplicación, ya que nos brinda una perspectiva directa de las experiencias, necesidades y sugerencias de aquellos que están utilizando activamente nuestra plataforma en su fase inicial.

## 2. Sprint 2
En el Sprint 2, la aplicación desplegada junto al formulario (definido en el documento **pilots.md**) se entregó el 25 de marzo. Posteriormente, el formulario se cerró el 27 de marzo para el grupo de tarde y el 2 de abril para Manos Abiertas con Norte. Cabe destacar que se hizo un formulario para cada uno de los dos tipos de usuarios piloto.

### 2.1 Feedback del grupo 11
Según el commitment agreement de usuarios piloto con el grupo 11 de la tarde, serían 8 personas de cada grupo las que harían el testing. A 28 de marzo a las 00:00 solo obtuvimos 6 respuestas, con lo cual, el grupo 11 incumplió el acuerdo. Además, el grupoTambién cabe destacar que parte del feedback recibido no nos es de gran ayuda, ya que muestra que la información incluida en el formulario no fue leída con atención. Por ejemplo, mucho feedback corresponde a temas de autenticación de usuarios, cosa que en el formulario se indicó que aún no estaba implementada. Aún así, este es el feedback recibido:
#### General
###### Errores
- Arreglar la visibilidad de la versión móvil.
- Habría que limitar caracteres en campos de texto, ya que si se introducen demasiados, el formulario se acaba rompiendo.
###### Sugerencias
- En general, revisar la ortografía.
- Adaptar el nombre de la pestaña de la aplicación.
#### Página de inicio
###### Errores
- En el formulario de "Donaciones puntuales", no hay validaciones de datos. Por ejemplo, se pueden meter valores numéricos en nombre y apellido.
###### Sugerencias
- En el footer, poner los números de teléfono de manera más lejible. Por ejemplo, 650 485 214 ó 650 48 52 14.
- En la sección "Asociación", la imagen tiene una resolución demasiado baja.
- En la sección "Donde estamos", sería conveniente cambiar las imágenes de los mapas por mapas interactivos.
#### Panel de administrador
###### Errores
- En general, los formularios de creación/edición no muestran errores específicos, con lo cual, no se puede saber que es lo que está mal.
###### Sugerencias
- En general, cuando se hace alguna operación CUD a cualquier instancia, podría aparecer algún tipo de mensaje como "Instancia creada/editada/borrada con éxito", ya que es confuso que se quede en la misma página. Esto podría causar una doble operación a alguna instancia.
##### Gestión de voluntarios
###### Errores
- Fotos no cargan. 
- Elementos no reactivos (agrandar y minimizar la ventana no tiene efecto en los elementos).
- La edición de voluntarios no funciona.
###### Sugerencias
- Header podría hacerse más pequeño, ocupa demasiado espacio.
- Se podría mostrar un mensaje como "No tiene solicitudes" si no las hay.
##### Gestión de educadores
###### Errores
- Las validaciones del form de "Añadir educador" no son detalladas. No se sabe cuales de los campos son los que están incorrectos.
###### Sugerencias
- "Añadir educador" podría ser un botón y no una sección.
##### Gestión de socios
###### Errores
- Se pueden crear asambleas en el pasado.
- Al crear una asamblea, el campo de hora debería ser una hora.
- Ahora mismo, en "Convocar asambleas" los campos no tienen límite de caracteres, con lo cual, con una cantidad muy grande de caracteres, el formulario se rompe y lanza una Bad Request, pero visualmente, no muestra ningún error.
###### Sugerencias
- "Convocar asamblea" podría ser un botón y no una sección.
- En "Convocar asamblea", el campo descripción podría ser un campo de texto más grande.
##### Gestión de clases
###### Errores
- En "Crear clase", se permite crear una clase con un minuto diferencia entre el inicio y el fin, y permite poner capacidad 0.
- Los errores de validación de datos de "Crear clase" no son específicos y/o no se corresponden con el fallo.
- Al darle a editar a una clase:
	- El formulario no contiene las fechas de la clase. 
	- No aparecen bien los educadores.
	- Errores de validaciones de datos no descriptivos.
###### Sugerencias
- Sería conveniente que al seleccionar que la clase sea de mañana o de tarde, los estudiantes se filtren automáticamente.

##### Gestión de eventos
###### Errores
- Limitar la creación de eventos. Se puede romper muy fácilmente.
- Al editar un evento, éste desaparece del calendario y hay que refrescar la página para que vuelva a salir.
###### Sugerencias
- Ajustar el estilo del calendario a la página, ya que desentona un poco.
##### Gestión de sugerencias
###### Errores
- Al no tener límite de caracteres al crear una sugerencia, si hay demasiado texto, éste se sale del cuadro azul. Es decir, no hay salto de línea.
#### Página de voluntario
###### Sugerencias
- En general, añadirle funcionalidad.
#### Página de socio
###### Sugerencias
- En general, añadirle funcionalidad.
#### Página de sugerencias
###### Errores
- El error de validación en el aviso de asunto no introducido tiene un error gramatical.
###### Sugerencias
- Limitar el número de caracteres.

#### Rendimiento
- Hay un archivo CSS externo que retrasa la visualización de la página en la ruta `/static/css/main.9b467832.css`.
- El **LCP** (Largest Content Page) es alto, se debe a que el HTML tiene mucho texto.
- Hay ocho recursos que no se entregan a través de una red **CDN**. Sería conveniente que se hiciera por CDN para que los archivos carguen más rápido. Estos ocho recursos son:
	- https://nexong.ew.r.appspot.com/static/js/main.6477887a.js
	- https://nexong.ew.r.appspot.com/static/css/main.9b467832.css
	- https://nexong.ew.r.appspot.com/static/media/macn-logo.aea120b27322
ad11cf16.png
	- https://nexong.ew.r.appspot.com/static/media/manosabiertas.f84baedec
c53eab2b8e1.png
	- https://nexong.ew.r.appspot.com/favicon.ico
	- https://nexong.ew.r.appspot.com/manifest.json
	- https://nexong.ew.r.appspot.com/logo192.png
	- https://nexongapi.ew.r.appspot.com/api/
- La **configuración de caché** no está optimizada para los mismos ocho recursos del punto anterior.
- Se ha identificado un problema de desplazamientos inesperados del contenido
en la página, lo cual puede afectar negativamente la experiencia del usuario. El
indicador **Cumulative Layout Shift (CLS)**, que mide la estabilidad visual de la
página, ha registrado un valor de 0.777, indicando movimientos significativos en
el diseño. Este problema parece estar causado por al menos una imagen crítica
para el diseño que no tiene definido un ratio de aspecto, específicamente la
imagen ubicada en `/static/media/macn-logo.aea120b27322ad11cf16.png`. Sin un
ratio de aspecto predefinido, el navegador no puede reservar el espacio
adecuado para la imagen antes de que se cargue completamente, resultando en
cambios inesperados en el layout a medida que se descarga la imagen.

#### Seguridad
- La versión HTTP de la página debería redirigir automáticamente a la versión HTTPS.

Estas son las seis personas del grupo 11 que hicieron de usuarios pilotos:

| Nombre                    | Correo US             | Fecha en que se recepciona el  acceso al sistema | Fecha en la que  envió el feedback | Link de Clockify                                        |
|---------------------------|-----------------------|--------------------------------------------------|------------------------------------|---------------------------------------------------------|
| LAURA ROLDÁN MERAT        | laurolmer@alum.us.es  | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/6606c4a26cf4e742fab3dc35)                                                        |
| MARIO AROCA PÁEZ          | mararopae@alum.us.es  | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/66042df1d153242e8bd7898b) |
| ISMAEL RUIZ JURADO        | ismruijur@alum.us.es  | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/66042e37d153242e8bd78aee) |
| PEDRO JESUS RUIZ AGUILAR  | pedruiagu1@alum.us.es | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/66042f59d153242e8bd78fe2) |
| JUAN CARLOS RAMIREZ LOPEZ | juaramlop2@alum.us.es | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/660461dae2d3e843b7baf0b9) |
| VIRGILIO OLIVA ALONSO     | virolialo@alum.us.es  | 25/03/2024                                       | 27/03/2024                         | [Link](https://app.clockify.me/shared/660497f3e2d3e843b7bb7b89) |

### 2.2 Feedback de Manos Abiertas con Norte
A continuación, exponemos el feedback dado por nuestro cliente, Manos Abiertas con Norte:
#### General
- Nos piden especial atención a la visibilidad móvil, ya que es lo que los usuarios usan principalmente.
- También nos piden atención al panel para educadores y autorizaciones de salidas para niños.
#### Página de inicio
###### Errores
- En el header, donde pone `Agenda`, debería poner `Agenda 2030`.
- En el footer:
	- Polígono norte debe estar escrito como `Polígono Norte`.
	- Añadir el teléfono del local viejo, que es `660 980 483`.
	- Añadir el CIF, que es `G-41753435`.
	- En general, mirar el footer de su actual página e incluir todo.

#### Panel de administrador
##### Gestión de voluntarios
###### Errores
- En las solicitudes, al darle al botón `Descargar` no descarga nada.
- El administrador debería poder editar a los voluntarios.

##### Gestión de educadores
###### Sugerencias
- En cada educador, en su vista previa, podría aparecer una descripción de los educadores en la que escriban quienes son y su horario. También podría aparecer la fecha de nacimiento.

##### Gestión de socios
###### Errores
- No se descargan las donaciones.

###### Sugerencias
- En cada socio, en su vista previa, también podría aparecer una pequeña descripción.

##### Gestión de clases
###### Errores
- Debería dejar asignar clases a educadores.
##### Gestión de eventos
###### Errores
- Debería dejar inscribir a ciertos participantes dependiendo del día y no para todo el evento. Por ejemplo, si un evento tiene lugar el 1, el 2 y el 3 de junio, puede ser que un educador pueda el 1, otro el 2 y otro el 3. _Después de la reunión del 05/04, se ha llegado al acuerdo de que al crear eventos, se cree un evento por día (aunque dure varios) y los usuarios se apuntarán al día que sea dependiendo de su disponibilidad_.
- Al crear/editar un evento no te debería de dejar meter a estudiantes, ya que ellos son los que se apuntan desde las cuentas familiares.

Esta es la información de nuestros usuarios piloto:

| Nombre | Correo | Fecha en que se recepciona el  acceso al sistema | Fecha en la que envió el feedback | 
|---------------------------|--------------|--------------------------------------------------|------------------------------------|
| MARÍA ARCE        |manosabiertas@lasalleandalucia.net| 25/03/2024                                       | 03/04/2024                         |

### 2.3 Futuros cambios
Respecto al feedback recibido por parte del grupo de tarde, habrá una tarea durante el Sprint 3 que será la mitigación de errores y la implementación de sugerencias. El feedback general y el seguridad se tendrán completamente en cuenta en el desarrollo de dicha tarea. Sin embargo, en el rendimiento no se tendrán en cuenta el LCP y el CLS, pero se investigarán las otras cuestiones.

Respecto al feedback recibido por parte de Manos Abiertas con Norte, se tendrá en cuenta todo. Se hará durante el resto del Sprint 3.

## 3. Sprint 3
En el Sprint 3, la aplicación desplegada junto al formulario (definido en el documento **pilots.md**) se entregaron el 14 de abril. Posteriormente, el formulario se cerró el 18 de abril para el grupo de tarde y el 22 de abril para Manos Abiertas con Norte. Cabe destacar que se hizo un formulario para cada uno de los dos tipos de usuarios piloto, al igual que en el Sprint 2.

### 3.1 Feedback del grupo 11
Según el commitment agreement de usuarios piloto con el grupo 11 de la tarde, serían 7 personas de cada grupo las que harían el testing. Se han recibido 7 respuestas antes del cierre del formulario, sin embargo, el grupo 11 no entregó su despliegue a tiempo, con lo cual, han vuelto a incumplir nuestro commitment agreement. Este es el feedback recibido:
#### Página de inicio
###### Errores
 - Para las personas que lo probaron el 15 de abril les salía error de CORS. Esto fue arreglado pronto, pero esas personas no pudieron probarlo bien.
 - En el registro de voluntarios, a veces salen los errores de validaciones y otras no.
 - En la sección *Asociación* los textos se "buguean" cuando se recarga la página.
 - En la sección *Entidades* las imágenes no cargan.
 - Hay fallos 500 al inspeccionar la consola.
 - Los errores tipo "toast" salen blanco sobre blanco, no se puede leer cual es el error.
 - Quitar el botón de inicio de sesión con Google si no se va a implementar.
###### Sugerencias
- Revisar ortografía de nuevo. Por ejemplo, `Dónde estamos` debería ser `Donde estamos`.
- En *Historia*, la imagen tiene mala calidad, considerar poner otra fotografía o reducir su tamaño.
- En *Club de verano*, el texto del cuadro de CLUB DE VERANO no está centrado como el resto de páginas.
#### Panel de administrador
##### Perfil
###### Errores
- Salta un error 400 al editar.
- No hay errores de validación.
##### Gestión de voluntarios
###### Errores
- Cuando se actualiza a un voluntario, redirige al perfil del administrador.
- Deja poner caracteres numéricos como nombre o apellido.
- Los errores de validaciones son blanco sobre blanco y no se pueden ver.
##### Gestión de educadores
###### Errores
- En la edición de educadores, redirige al perfil del administrador también.
- No hay mensajes de validaciones.
- Al crearlos, da un error 400.
- Deja poner caracteres numéricos como nombre o apellido.
- Los errores de validaciones son blanco sobre blanco y no se pueden ver.
##### Gestión de socios
###### Errores
- En la edición de socios, redirige al perfil del administrador también.
- Deja poner caracteres numéricos como nombre o apellido.
- En la descarga de socios, cuando eliges un formato, se descarga bien, pero, si eliges la opción "Formato a descargar" salta un error 404.
##### Gestión de familias
###### Errores
- Si aceptas una solicitud, el mensaje que sale es `Persona rechazada correctamente`.
##### Gestión de clases
###### Errores
- Mismos errores que en el Sprint 2.
- Los errores de validaciones son blanco sobre blanco y no se pueden ver.
##### Gestión de eventos
###### Errores
- Los eventos desaparecen al ser editados, hay que recargar la página para verlos.
- No hay errores de validaciones.
##### Gestión de documentos
###### Errores
- Permite poner fechas muy extremas, como 1000 o 4000.
- No se muestran en la página de *Transparencia* una vez creados.
#### Registro de voluntarios
###### Errores
- No ha funcionado para algunos de ellos.
#### Registro de familias
###### Errores
- No ha funcionado para algunos de ellos.
- El token y los términos y condiciones no deberían verse por consola.
- No hay mensajes de errores de validación.

#### Sugerencia interesante de uno de los usuarios pilotos
- Creo que el responsiveness de la pagina podría estar mas pulido. Hay paginas que en la versión móvil se ven regular, sobre todo por el header. Quizás sería mejor idea para el header y las secciones implementar un menú de hamburguesa que se despliegue en vez de comprimirlas todas.  Después en las pantallas grandes la aplicación ocupa todo el ancho de la pantalla, lo cual no es muy cómodo, podría ser buena idea utilizar media queries de css para acotar las paginas para tener una anchura máxima (https://www.freecodecamp.org/news/media-query-css-example-max-and-min-screen-width-for-mobile-responsive-design/)

Estas son las siete personas del grupo 11 que hicieron de usuarios pilotos:

| Nombre                    | Correo US             | Fecha en que se recepciona el  acceso al sistema | Fecha en la que  envió el feedback | Link de Clockify                                        |
|---------------------------|-----------------------|--------------------------------------------------|------------------------------------|---------------------------------------------------------|
| LAURA ROLDÁN MERAT        | laurolmer@alum.us.es  | 15/04/2024                                       | 15/04/2024                         | [Link](https://app.clockify.me/shared/661d67378b3afb4fb192e682)                                                        |
| MARIO AROCA PÁEZ          | mararopae@alum.us.es  | 15/04/2024                                       | 17/04/2024                         | [Link](https://app.clockify.me/shared/661fe9600730fe5f66b4b47e) |
| ISMAEL RUIZ JURADO        | ismruijur@alum.us.es  | 15/04/2024                                       | 16/04/2024                         | [Link](https://app.clockify.me/shared/661e953580edc7302cbe6070) |
| PEDRO JESUS RUIZ AGUILAR  | pedruiagu1@alum.us.es | 15/04/2024                                       | 16/04/2024                         | [Link](https://app.clockify.me/shared/661e96e7ea745f2d088db700) |
| IVAN SANCHEZ SANJOSE    | ivasansan1@alum.us.es  | 15/04/2024                                       | 15/04/2024                         | [Link](https://app.clockify.me/shared/660497f3e2d3e843b7bb7b89) |
| JOSE JAVIER ALCOBENDAS SANTOS    | josalcsan1@alum.us.es  | 15/04/2024                                       | 16/04/2024                         | [Link](https://app.clockify.me/shared/6620df3880edc7302cc41155) |
| VIRGILIO OLIVA ALONSO    | virolialo@alum.us.es  | 15/04/2024                                       | 17/04/2024                         | [Link](https://app.clockify.me/shared/66200c5180edc7302cc27b21) |

### 3.2 Feedback de Manos Abiertas con Norte
Aún no se ha recibido feedback.

### 3.3 Futuros cambios
Respecto al feedback recibido por parte del grupo 11, será abordado durante la semana de retrospectiva entre el Sprint 3 y el PPL.
