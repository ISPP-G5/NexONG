# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Documento de requisitos - Sprint 1


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

1. Clasificación por Roles
2. Requisitos generales



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
   <td>09/02/24</td>
   <td>Primer borrador</td>
  </tr>
  <tr>
   <td>1.0.1</td>
   <td>10/02/24</td>
   <td>Versión revisada (@fracalrod3)</td>
  </tr>
  <tr>
   <td>1.1.0</td>
   <td>01/03/24</td>
   <td>Versión revisada tras segunda reunión con la ONG</td>
  </tr>
</table>


<br/>

# 

<br/>

 
# 1. Clasificación por Roles

Los usuarios tendrán roles, y por lo tanto acceso a:

- **Administrador**
    - Visualización de toda la información así como el estado de cursos, eventos, donaciones y usuarios(educadores, alumnos, voluntarios y socios) en tiempo real.
    - Creación y borrado de cursos que contendrá fecha de inicio y de fin del curso.
    - Creación y asignación de educadores a cursos.
    - Creación, modificación y borrado de centros educativos.
    - Asignación de alumnos a cursos (son los familiares los que tendrán acceso a este usuario).
    - Volcado de información a archivos estándar (.xlsx, .pdf, .csv).
    - Creación de asambleas(solo asisten la junta directiva y los socios).
    - Creación de eventos (puede tener un límite de plazas tanto de alumnos como de voluntarios).
    - Creación de eventos puntuales asociados a cursos (puede tener un límite de plazas).
    - Creación y modificación de proyectos
        - Los proyectos consisten en título, descripción y cosas a evaluar del proyecto, así como las personas asociadas a ellos(educadores).
    - Ver las evaluaciones trimestrales y anuales de dichos proyectos.
    - Asignación de al menos 1 educador a un evento o evento puntual, donde contará con privilegios (tal y como si fuera un curso).
    - Aceptación o rechazo de alumnos de tarde y de voluntarios.
- **Educador/Profesor**
    - Control de asistencia diario de alumnos inscritos en su curso.
    - Evaluación diaria de alumnos a través de categorías establecidas por el administrador.
    - Creación de observaciones y comunicaciones dirigidas a los familiares (personales) .
    - Creación de boletines de evaluación trimestrales y finales dirigido a los familiares.
- **Centros Educativos**
    - Adjuntar y mandar información para inscribir a un niño.
    - Adjuntar información de las actividades que tiene que realizar el niño durante su expulsión.
    - Recibir informes del niño como si fuese un familiar(evaluación diaria y final).
- **Familiar/es**
    - Formulario de documentación para dar de alta al alumno (esta debe de ser aprobada por el administrador)
    - Visualización de próximos eventos e inscripción a estos (algunos pueden ser de pago).
    - Visualización de evaluación diaria del alumno.
    - Visualización de observaciones y comunicaciones dirigidas al alumno.
    - Visualización de boletines de evaluación finales del alumno.
    - Visualización de las próximas clases en un calendario así como los próximos eventos importantes (que deberán incluirse también en un tablón especial).
    - Inscripción a la participación en los eventos y eventos puntuales que tenga disponible el alumno (ej.: un alumno de primaria no puede inscribirse a un evento de infantil, pero un alumno de primaria si puede inscribirse a un evento dirigido a todos los cursos).
    - Formulario de documentación para incluir trimestralmente el boletín de notas proporcionado por el colegio.
    - En el caso de que sea la familia de un niño inscrito por el centro escolar, podrá acceder a las mismas áreas que una familia normal, solo cambiará la documentación inicial y el proceso de inscripción.
- **Voluntario**
    - Inscripción a la participación en cursos un día concreto como soporte del educador (En calendario o tablón especial).
    - Visualización de la asistencia total a cursos y eventos, así como de las ausencias en eventos o cursos en los que se haya apuntado.
- **Socios**
    - Formulario de documentación para adjuntar la documentación relativa a las cuotas mensuales y abonos puntuales.
    - Visualización e historial de dichas cuotas y abonos.
    - Visualización del calendario y el tablón con eventos relevantes, así como las asambleas.
    - Visualización de la asistencia a asambleas.


# 2. Requisitos generales

- Debe ser una interfaz sencilla y de uso fácil, ya que la mayoría de personal no posee conocimientos informáticos avanzados.
- Debe tener capacidad para el uso simultáneo de 50-100 personas.
- Debe ser un sistema escalable, admitiendo como mínimo 250 usuarios, siendo expandible en el futuro.
- Todos los eventos y eventos puntuales publicados por el administrador, deben también ser recibidos mediante correo electrónico, conteniendo un enlace de acceso directo a la plataforma.
- La aplicación debe contener una sección de noticias, que debe reenviar la información vía e-mail, conteniendo un enlace de acceso directo a la plataforma.
- Los usuarios pueden procesar la baja de noticias en el e-mail.
- La aplicación debe contener una cláusula de privacidad y manipulación de datos según la legislación vigente.
- Debe ser compatible la posibilidad de tener el rol de Voluntario y Socio al mismo tiempo.
- Debe tener total prioridad la administración educativa, seguidamente la gestión de voluntarios y por último la de socios.
- La homepage debe contener pantallas obligatorias como todas las relativas a la organización, transparencia, visión, misión, entidades colaboradoras, o la agenda 2030.
- Para la parte de transparencia se deben de almacenar los programas de años anteriores, así como añadir los nuevos.
