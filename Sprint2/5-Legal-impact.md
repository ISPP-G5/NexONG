# Impacto Legal del Proyecto - Sprint 2
# Nexong - Grupo 5

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
2. Leyes de protección de datos
3. Seguridad de datos
4. Confidencialidad y privacidad
5. Responsabilidad legal
6. Consentimiento de los padres/tutores


## Registro de cambios

<table>
  <tr>
   <td><strong>Versión</strong>
   </td>
   <td><strong>Fecha</strong>
   </td>
   <td><strong>Descripción</strong>
   </td>
   <td><strong>Participantes</strong>
   </td>
  </tr>
  <tr>
   <td>1.0.0</td>
   <td>16/3/2024</td>
   <td>Primera versión</td>
   <td>
     Redacción: FRANCISCO DE ASÍS ROSSO RAMÍREZ Revisión: CLAUDIA GILABERT PRIETO
   </td>
  </tr>
  <tr>
    <td>1.1.0</td>
    <td>25/3/2024</td>
    <td>
      <ul>
        <li>Ampliación del apartado 3</li>
        <li>Corrección de erratas</li>
      </ul>
    </td>
    <td>
      Redacción: FRANCISCO DE ASÍS ROSSO RAMÍREZ Revisión: AURORA NAVAS JIMÉNEZ
    </td>
  </tr>
</table>


<br/>

# 

<br/>


# 1. Introducción
El presente documento recoge las consideraciones legales a tener en cuenta durante el desarrollo de la aplicación web para la ONG Manos Unidas con Norte por parte de la organización NexONG, cuya finalidad es proporcionar a la mencionada ONG una herramienta de administración y gestión de los datos con los que deben tratar, tales como pueden ser alumnos apuntados, clases, actividades, voluntarios o donaciones. Se contemplan temas inherentes al trato de información personal, como protección y seguridad de datos, así como relativos al trabajo con menores de edad.

# 2. Leyes de protección de datos
Como país miembro de la Unión Europea, estamos sujetos al Reglamento General de Protección de Datos (RGPD), vigente desde el 27 de abril de 2016, que rige la recopilación y el tratamiento de datos personales de los usuarios para compañías establecidas en la UE, sin importar si el tratamiento se hace dentro o fuera de esta, así como compañías no establecidas en la UE ofreciendo bienes o servicios dentro de la UE o a individuos de la UE.

Además, en España está vigente la Ley Orgánica de Protección de Datos y Garantía de Derechos Digitales (LOPDGDD), que sustituyó en diciembre de 2018 a la antigua Ley Orgánica de Protección de Datos (LOPD) adaptándola a todo el contendio del reglamento europeo y extendiéndolo, de forma que cumpliendo la LOPDGDD se estará cumpliendo también la RGPD.
Entre las diferencias, podemos encontrar en la LOPDGDD las siguientes ampliaciones de la RGPD:
- Se eleva la edad de consentimiento de un menor de 13 a 14 años.
- Amplía los individuos que pueden acceder a los datos de personas fallecidas.
- Amplía los derechos digitales.
- Otorga una mayor precisión a la hora de exponer las infracciones y la cuantía legal de las mismas.
- Expone los casos concretos en los que una empresa debe designar un delegado de protección de datos.

# 3. Seguridad de datos
La seguridad de los datos es una preocupación fundamental para NexONG, dada su responsabilidad como custodio de la información personal de los niños, familias y voluntarios. Para garantizar la seguridad de estos datos, es crucial implementar medidas técnicas y organizativas sólidas; de esta forma contaremos con:
- **Control de acceso**. Implementar un sistema de control de acceso robusto, basado en roles y privilegios, que garantice que solo personal autorizado tenga acceso a la información relevante. Lo llevaremos a cabo mediante la autenticación de usuarios y la implementación de políticas de acceso basadas en el principio de "menos privilegios", donde cada usuario tenga acceso exclusivamente a la información necesaria para llevar a cabo sus funciones. Los roles con los que contará nuestro sistema son:
    - **Socio**. Dona periódicamente a la organización y puede ir a asambleas convocadas por la junta directiva.
    - **Familia**. Corresponde a la cuenta de un familiar o tutor legal de un menor registrado como alumno.
    - **Voluntario**. Ayuda a la ONG colaborando con los educadores en actividades y clases.
    - **Educador**. Trabajadores fijos de la organización, se encargan de los alumnos y llevan a cabo las actividades y clases.
    - **Administrador**. La figura principal de la organización, lleva el control de todos los datos y acontecimientos.
- **Plan de respuesta ante incidentes**. Disponer de un plan de respuesta ante incidentes para actuar de manera rápida y eficiente en caso de acceso no autorizado a los datos. Este constará de los siguientes procedimientos:
    - **Procedimientos de notificación**. Notificar a las partes pertinentes sobre cualquier incidente de seguridad.
    - **Investigación y evaluación**. Investigación exhaustiva para determinar la naturaleza y el alcance del incidente de seguridad.
    - **Mitigación de riesgos**. Medidas inmediatas para mitigar los riesgos asociados con el incidente de seguridad, entre las que se encuentran la desconexión de sistemas comprometidos y la restauración de copias de seguridad limpias.
    - **Evaluación post-inicidente**. Evaluación exhaustiva tras el incidente para identificar lecciones aprendidas y áreas de mejora en el plan de respuesta.
 
# 4. Confidencialidad y privacidad
Se deberá garantizar la confidencialidad de todos los datos almacenados en la aplicación. Para ello debemos considerar:
- **Políticas y procedimientos claros**. Establecer políticas y procedimientos claros para garantizar la confidencialidad de los datos almacenados en la aplicación web. Entre estas medidas destacamos:
    - Definición clara de quiénes tienen acceso a qué información.
    - Cómo se protege la información contra el acceso no autorizado.
    - Qué medidas se tomarán para proteger la seguridad de la información.
      \
Todo esto será controlado por el sistema de roles y privilegios, que nos permite controlar mediante registro regulado por documentos el acceso de cada usuario a la información, protegiendo del resto partes confidenciales o más restringidas.
- **Formación y sensibilización**. Es crucial el conocimiento del personal de NexONG sobre la importancia de la confidencialidad y privacidad de los datos, por lo que se podrá llevar a cabo formación al respecto si se considera necesario.
- **Confianza y transparencia**. NexONG debe establecer relaciones de confianza con sus usuarios, lo que implica una información transparente acerca de la recopilación, uso y almacenamiento de los datos, así como permitir a los usuarios ejercer sus derechos de acceso, rectificación, supresión y oposición de los datos.

# 5. Responsabilidad legal
NexONG es responsable de los datos almacenados en su aplicación, y por tanto encargada de garantizar su seguridad y su privacidad.
Las ONG que hagan uso de la aplicación son responsables del mismo, con lo que NexONG no se hace responsable de cualquier uso incorrecto.

# 6. Consentimiento de los padres/tutores
Los padres o tutores legales deberán ser completamente informados de qué datos se almacenan en la aplicación web de NexONG, con qué finalidad serán recogidos y qué se hará con ellos.
