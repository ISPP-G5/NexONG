# Feedback de los usuarios pilotos - Sprint 2
# NexOng - Grupo 5

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


## Registro de cambios

| Versión | Fecha | Descripción | Participantes |
|---------|-------|-------------|---------------|
|1.0.0|28/03/2024|Feedback del Sprint 2|Redacción: AURORA NAVAS JIMÉNEZ Revisión: MARÍA NÚÑEZ REYES|
|1.0.1|30/03/2024|Cambio de portada según failure conditions|Redacción: AURORA NAVAS JIMÉNEZ Revisión: MANUEL ORTIZ BLANCO y PEDRO LÓPEZ RUZ|


## 1. Introducción
El presente documento tiene como objetivo principal recopilar y analizar el valioso feedback proporcionado por los usuarios pilotos, previamente definidos en el documento **5-Pilot-Users**. Este proceso de retroalimentación juega un papel fundamental en el desarrollo y mejora continua de nuestra aplicación, ya que nos brinda una perspectiva directa de las experiencias, necesidades y sugerencias de aquellos que están utilizando activamente nuestra plataforma en su fase inicial.

## 2. Sprint 2
En el Sprint 2, la aplicación desplegada junto al formulario (definido en el documento **5-Pilot-Users**) se entregó el 25 de marzo. Posteriormente, el formulario se cerró el 27 de marzo para el grupo de tarde y el 2 de abril para Manos Abiertas con Norte. Cabe destacar que se hizo un formulario para cada uno de los dos tipos de usuarios piloto.

### 2.1 Feedback del grupo 11
Según el commitment agreement de usuarios piloto con el grupo 11 de la tarde, serían 8 personas de cada grupo las que harían el testing. A 28 de marzo a las 00:00 solo obtuvimos 6 respuestas, con lo cual, el grupo 11 incumplió el acuerdo. También cabe destacar que parte del feedback recibido no nos es de gran ayuda, ya que muestra que la información incluida en el formulario no fue leída con atención. Por ejemplo, mucho feedback corresponde a temas de autenticación de usuarios, cosa que en el formulario se indicó que aún no estaba implementada. Aún así, este es el feedback recibido:
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
Se les envió el formulario y el despliegue el 25 de marzo, pero Manos Abiertas con Norte aún no han hecho de usuarios piloto. Entendemos que son una organización ocupada y que no tienen un horario flexible. Al ser su feedback tan importante para nosotros, se les dará más márgen.

### 2.3 Futuros cambios
