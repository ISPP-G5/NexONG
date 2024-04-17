# Changelog - Sprint 3
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
2. Incrementos (Features)
3. Mejoras (Improvements)
4. Arreglos (Fixes)


## Registro de cambios


<table>
  <tr>
   <td><strong>Versión</strong>
   </td>
   <td><strong>Fecha</strong>
   </td>
   <td><strong>Descripción</strong>
   </td>
   <td><strong>Redacción</strong>
   </td>
   <td><strong>Revisión</strong>
   </td>
  </tr>
  <tr>
   <td>1.0.0</td>
   <td>11/4/2024</td>
   <td>Primera versión</td>
   <td>FRANCISCO DE ASÍS ROSSO RAMÍREZ</td>
   <td></td>
  </tr>
</table>



<br/>

# 

<br/>



#  1. Introducción

En este documento se recogen los avances realizados en el proyecto durante el desarrollo del Sprint 3,
divididos en: incrementos o *features* (nuevas características del proyecto), mejoras o *improvements*
(continuación del desarrollo de partes de código ya hechas anteriormente para actualizarlas o
proporcionarles una mejor utilidad) y arreglos o *fixes* (reparación de partes del código que no
funcionaban correctamente o se han quedado obsoletas). Cada apartado se desglosa en las partes *backend*
y *frontend*.



# 2. Incrementos (Features)


## 2.1 Backend


### Feature/78-Export Partner/Partners data

Creación de un CSV, un PDF y un Excel de los datos seleccionados del backend, dando también la opción
de descargar los archivos relacionados en un archivo comprimido zip o rar o mediante una URL.


### Feature/79-Export Volunteers/Volunteer data

Creación de un CSV, un PDF y un Excel de los datos seleccionados del backend, dando también la opción
de descargar los archivos relacionados en un archivo comprimido zip o rar o mediante una URL.


### Feature/80-Export Students/Student data

Creación de un CSV, un PDF y un Excel de los datos seleccionados del backend, dando también la opción
de descargar los archivos relacionados en un archivo comprimido zip o rar o mediante una URL.


### Feature/135-Terms

Añadido al modelo de una tabla que registra quién ha aceptado qué versión de los términos y condiciones.


### Feature/137-Load tests

Creación de los tests de carga.


### Feature/138-Tests for admin

Creacioón de los tests unitarios de usuarios administradores.


### Feature/139-Tests for partner

Creación de los tests unitarios de usuarios socios.


### Feature/140-Tests for student & family

Creación de los tests unitarios de usuarios familia/alumno.


### Feature/141-Tests for volunteer

Creación de los tests unitarios de usuarios voluntarios.


### Feature/142-Tests for educator

Creación de los tests unitarios de usuarios educadores.


## 2.2 Frontend


### Feature/87-Volunteers Formation

Creación del segundo formulario para registro de voluntarios. Al terminar el registro como voluntario,
el usuario es redirigido a la pantalla de formación, con 3 vídeos.


### Feature/89-Volunteers Documentation

Una vez un nuevo voluntario ve los 3 vídeos, accede a la pantalla de documentación, donde descarga y
envía los documentos necesarios para enviar su solicitud.


### Feature/120-Admin volunteers docs

Añadido botón para que un administrador pueda descargar un zip con todos los documentos entregados
por un voluntario al rellenar su formulario.


### Feature/161-Payment system

Añadida la parte frontend para el sistema de pago implementado en backend.


### Feature/165-Recurring donations

Ahora es posible registrarse como socio desde la pantalla "Registrarse"; hay que completar un segundo
formulario para los datos que faltan. Rediseño de la pantalla "Donaciones" para volverla *responsive*
y reducir la parte de donaciones recurrentes.


### Feature/166-Privacy policy

La casilla para aceptar los términos de privacidad incluye ahora un enlace a los mismos.


### Feature/167-Family daily and yearly evaluation

Las familias ahora pueden ver los resultados de las evaluaciones diarias y anuales de sus niños.


### Feature/168-Family authorizations

Las familias pueden firmar autorizaciones para sus niños.


### Feature/169-Family kids

Las familias pueden ver a sus niños y apuntar nuevos.


### Feature/170-Family calendars

Las familias pueden acceder a un calendario con clases, eventos y actividades


### Feature/171-Registration of families

Es posible registrarse como familia desde la pantalla "Registrarse"; hay que completar dos formularios
más para la información restante.


### Feature/179-Home page La Salle

Añadida información a la pantalla "La Salle".


### Feat/191-Partners membership

Los socios ahora pueden modificar la cantidad que donan y actualizar y cancelar su afiliación.


### Feat/204-Schedule for classes

Ahora las clases tienen un horario.


# 3. Mejoras (Improvements)


## 3.1 Backend


### Feature/133-Feedback of pilots users

Implementación del feedback proporcionado por los usuarios piloto:
- Al borrar un socio, sus donaciones ya no se eliminan.
- Al borrar un educador, las clases asociadas a este ya no se se eliminan.
- La fecha de una reunión no puede estar en el pasado ahora.
- Educador y socio tienen un campo de descripción
- Añadida redirección de HTTP a HTTPS solo para el entorno de producción. HTTPS no está disponible para
el entorno de desarrollo.


### Feature/154-Log in and register with token

Implementada autenticación mediante tokens.


### Feature/134-Change in models

Cambios en los modelos de datos. Estos son:

- Limitar el máximo de caracteres en algunos campos.
- Habilitar el modelo y CRUD de horario.
- Habilitar un campo en el usuario para almacenar si este ha aceptado los términos y condiciones y qué
versión de estos.
- La verificación por email se resuelve en backend.

## 3.2 Frontend


### Fix/144-Information main page of home page

Añadida la información de la página principal.


### Fix/145-About us video and dossier

Añadidos vídeo y dosier en la pantalla "Nosotros".


### Fix/146-History home page

Añadida información a la pantalla "Historia"


### Fix/147-Mission, view and values

Añadida información a la pantalla "Misión, Visión y Valores".


### Fix/148-Association information

Añadida información a la pantalla "Associación".


### Fix/149-Summer school

Añadida información a la pantalla "Campamento de  verano".


### Fix/150-Update images

Actualizadas las imágenes de la aplicación con las proporcionadas por la ONG.


### Fix/151-Transparencies

Completada la tabla de la pantalla "Transparencia"


### Fix/163-Volunteers attendance

Ahora los voluntarios ven el nombre y tipo de actividad de las actividades a las que pueden unirse.


### Fix/172-Feedback pilot users

Implementación del feedback por parte de los usuarios piloto:
- Revisión de erratas.
- Cambio del nombre de la pestaña a Manos Abiertas.
- Teléfonos más visibles en el pie de página.
- Uso de mapas interactivos para "Dónde estamos".
- Mejores mensajes de error en formularios de administrador.
- Añadidos mensajes de éxito al borrar y editar.
- Voluntarios más pequeños en cabecera.
- Mensaje si no hay solicitudes en la pantalla de voluntarios para administradores.
- Mensajes de error de educadores más detallados.
- Cambio de añadir educador a un botón.
- Cambio de campo de tiempo a solo hora y no día.
- Mensaje de error en socios.
- Mensaje de error en clases.
- Los cambios aparecen inmediatamente al editar un evento.
- Cambios de estilo en el calendario.
- Eliminación de saltos de línea.
- Corrección de error gramatical en mensajes de error de sugerencias.


### Feature/175-Social log in

Ahora es posible iniciar sesión mediante Google.


### Fix/194-Log in and register

Ahora se puede crear una cuenta e iniciar sesión sin necesidad de utilizar la extensión Modheader.

# 4. Arreglos (Fixes)


## 4.1 Backend


### Fix/146-Fix user model

Al hacer POST de un usuario (registro) el frontend puede enviar el rol asociado. Solo se permite enviar
POST con rol de administrador o educador si el usuario es administrador.


### Fix/148-Fix user roles

Reparación del método POST de usuarios para que pueda volver a realizarse la operación. Un administrador
crea todos los modelos relativos a un usuario, y los demás roles solo crean los modelos que les
corresponden.

Arreglados los permisos de HomeDocument para que todos los usuarios puedan realizar operaciones tipo GET
pero solo los administradores puedan realizar POST, PUT y DELETE.


### Fix/151-Fix authentication systems

Reparación de problemas detectados con el sistema de autenticación implementado.


### Fix/155-Fix Lesson validator and add PATCH to User

Reparación de los validadores de clase para poder realizar operaciones POST. Añadida operación PATCH de
usuarios.


### Fix/157-Fix PunctualDonation permissions

Ahora todos los usuarios pueden realizar operaciones tipo POST a donaciones puntuales.


### Fix/159-Fix usable populate

Contraseñas de usuarios cambiadas a "contraseña" y cifradas con el sistema de Django para poder ser
testeadas desde frontend con populate.


### Fix/169-Fix download privileges

Ahora solo los administradores pueden descargar los archivos exportados tales como Exce, CSV y PDF (en
lugar de todos los usuarios, registrados o no).


### Fix/171-Fix email

Cambio del email de activación a español para poder ser entendido por los miembros de la ONG, inclusión
en el email de los siguientes pasos a realizar para continuar con el registro de la cuenta.


### Fix/173-Fix User PATCH/PUT

Ahora se puede editar un usuario.


## 4.2 Frontend


### Fix/162-Volunteers calendar

Ahora los voluntarios pueden apuntarse a clases y actividades además de eventos.


### Fix/164-Donations export

Ahora las donacinoes pueden ser exportadas en distintos formatos, no solo PDF.


### Fix/173-Admin families request

Los administradores pueden gestionar las solicitudes de familias. Tienen una lista de las familias
registradas en el sistema.


### Fix/174-Lesson event

Se han implementado arreglos y adiciones para funciones como admistrador.

En la pantalla "Clases":
- Añadidos botones y formularios para ver, crear, editar y borrar horarios.
- Añadida opción a la creación y edición de clases para indicar si es por la mañana.
- Ahora el educador y la fecha de cada clase aparecen en la pantalla "Clases".

En la pantalla "Eventos":
- Añadidos botones y formularios para crear, editar y borrar actividades.

### Fix/178-Delete projects, schools

Eliminados los campos relativos a proyectos y escuelas en el menú lateral de administrador


### Fix/185-Edit educators and volunteers

Ahora los administradores pueden editar y visualizar el perfil de educadores y voluntarios.


### Fix/190-Delete roles

Ahora se elimina el rol de un usuaro en lugar del usuario en sí.
