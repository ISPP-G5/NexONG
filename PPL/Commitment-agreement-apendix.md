# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Commitment Agreement Appendix - Sprint 3
# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NexOng - Grupo 5


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

1. Anexo al documento Commitment agreement
   1. Medidas de rendimiento de los miembros del equipo en la realización de código o documentación
   2. Rendimiento del S1
   3. Nota máxima de los miembros del equipo
   4. Formatos acordados en los repositorios de equipo
   5. Responsabilidades individuales en S1
   6. Rendimiento del S2
   7. Responsabilidades individuales en S2
   8. Rendimiento del S3
   9. Responsabilidades individuales en S3


## Registro de cambios

<table>
  <tr>
   <td><strong>Versión</strong>
   </td>
   <td><strong>Fecha</strong>
   </td>
   <td><strong>Descripción</strong>
   </td>
    </td>
   <td><strong>Redacción</strong>
   </td>
    </td>
   <td><strong>Revisión</strong>
   </td>
  </tr>
  <tr>
   <td>1.0.0</td>
   <td>29/2/2024</td>
   <td>Primera versión del anexo</td>
    <td>Pablo Periañez</td>
    <td>Marta Gonzalez</td>
  </tr>
  <tr>
   <td>2.0.0</td>
   <td>09/3/2024</td>
   <td>Cambio en la performance por solicitud del equipo</td>
    <td>Pablo Periañez</td>
        <td>Marta Gonzalez</td>
  </tr>
    <tr>
   <td>3.0.0</td>
   <td>21/3/2024</td>
   <td>Cambio en la formula por consistencia</td>
    <td>Pablo Periañez</td>
        <td>Marta Gonzalez</td>
  </tr>
  <tr>
   <td>4.0.0</td>
   <td>06/4/2024</td>
    <td>Cambio de los porcentajes de evaluación</td>
    <td>Pablo Periañez, Marta González</td>
    <td>Aurora Navas Jiménez</td>
  </tr>
  <tr>
   <td>5.0.0</td>
   <td>21/4/2024</td>
    <td>Añadir rendimiento del S3</td>
    <td>Pablo Periañez, Marta González</td>
    <td>Aurora Navas</td>
  </tr>
  <tr>
   <td>6.0.0</td>
   <td>21/4/2024</td>
    <td>Añadir rendimiento del PPL</td>
    <td>Pablo Periañez</td>
    <td>IVÁN RAMÍREZ LARA</td>
  </tr>
</table>


<br/>

# 

<br/>


# 1. Anexo al documento Commitment agreement

## Medidas de rendimiento de los miembros del equipo en la realización de código o documentación

Para calcular el rendimiento individual de los miembros del equipo se ha usado una estimación de tareas en poker planning. A cada número del poker planning se le asigna un duración en horas como estimación para esa tarea. A continuación se detallan las horas que se estiman para cada puntuación numérica del poker planning:

- 1 → 0.5 a 1 horas
- 2 → 1 a 1.5 horas
- 3 → 1.5 a 2 horas
- 5 → 2 a 3 horas
- 8 → 3 a 4 horas
- 13 → 4 a 6 horas
- 21 → 6 a 8 horas
- 34 → 8 a 10 horas

Al finalizar el Sprint se calculará el total de horas realizadas por ese miembro del equipo, en donde si se encuentra dentro del rango de horas estimado, la primera división tendrá un valor de 1. La formula para hacer el calculo sería:

$$\left(E_{total} = \sum_{i=0}^{n_{tareas} } \left( \frac{E_{realizado_i}}{E_{estimado_i}} \right)\right)$$

De cada Milestone, cada miembro del equipo contará con una calificación en referencia a su rendimiento en ese milestone y a la calidad de su trabajo. Esta medida de rendimiento constará de 3 partes fundamentales para cada miembro:

- **(C) Calificación de tareas:** Al final de cada milestone, los Team leader asignarán un número del 0 al 5, que simbolizará la calidad total del trabajo realizado por ese miembro. Cada Team leader solo lo asignará a los miembros de su equipo. Sin embargo habrá que tener en cuenta que:
  - Se podrá restar hasta 1 punto por cada problema grave implementado en código, o documentación en la que no se haya tenido en cuenta el feedback.
  - Se podrá restar hasta 1 punto si no se ha tenido en cuenta el orden a realizar las tareas o su prioridad asignada.
  - Se podrá restar hasta 1 punto si no ha realizado ninguna tarea de documentación en el Sprint.
- **(E) Esfuerzo:** Calculo estimado de la formula anterior dada la planificación del poker planning y las horas trabajadas.
- **(TNR) Tarea/s no realizadas:** Se tendrá en cuenta las tareas no realizadas o reasignadas a otros compañeros, que hayan alterado el flujo de trabajo normal del milestone. Este valor estará reflejado como la puntuación del poker planning de esas tareas no realizadas

Todas estas medidas conforman una fórmula que se aplicará a cada miembro del equipo para obtener su rendimiento personal durante todo el milestone:

$$\left(Perf_{total} = C \times (E - TNR) \right)$$

Posteriormente a calcular la calificación individual, se procederá a normalizar todos los valores en una escala del 0 al 5, tomando como referencia el mayor valor que la persona puede obtener en el Sprint dada su asignación de tareas. Esta nueva medida de rendimiento ponderará el 25% en la autoevaluación total, sustituyendo a la exterior del cálculo de horas proporcionado por Clockify.

**En el caso del Project Manager y los Team Leader, la calificación de tareas será sustituida por la puntuación que le asigne su equipo. Esto se hará mediante una pequeña encuesta donde solo participara el equipo de ese responsable.

Un 70% de la nota restante se obtendrá a través de un formulario de evaluación (Ev_Forms), que realizarán todos los miembros del equipo al final del sprint, en este se evaluarán aspectos subjetivos divididos en las siguientes secciones:
- **Contribución individual:** Aporte que cada miembro del equipo realiza al proyecto.
- **Colaboración:** Capacidad de la persona para trabajar efectivamente con otros miembros del equipo. 
- **Calidad del trabajo:** Nivel de contenido y precisión en las tareas realizadas.

Las secciones serán evaluadas del 1 al 5, siguiendo esta escalas de notas:
- **Insuficiente:** El objetivo no ha sido cumplido o está muy por debajo de lo que se esperaba.
- **Pasable:** El objetivo ha sido cumplido al mínimo y no ha sido del todo satisfactorio.
- **Aceptable:** El objetivo ha sido cumplido satisfactoriamente, cumpliendo con las expectativas.
- **Bien:** El objetivo ha sido cumplido de manera muy satisfactoria, alcanzando las expectativas establecidas.
- **Muy bien:** El objetivo ha sido cumplido superando las expectativas y todos los miembros del equipo han quedado muy satisfechos.

Una vez estén recolectados los datos se procesará una media aritmética sobre 10, tomando los valores:
- 1 → 4
- 2 → 6
- 3 → 7
- 4 → 9
- 5 → 10

El 10% restante de la nota se podrá consenguir mediantes bonificaciones por puntos de historia del Poker Planning o por ayuda a los compañeros. Pudiendo obtener hasta 2 puntos más si ambas fuesen perfectas. 
Para estos apartados se normalizarán las notas tomando la máxima puntuación como referencia.

$$\left(Nota_{final} = 0.7 \cdot Ev_{Forms} + 0.25 \cdot Perf_{total} + 0.1 \cdot Poker + 0.1 \cdot Ayuda \right)$$


## Rendimiento del S1

Según las medidas explicadas anteriormente, los miembros del equipo han obtenido la siguiente evaluación según el rendimiento durante el Sprint1:

<img width="615" alt="imagen" src="https://github.com/ISPP-G5/NexONG/assets/72883992/8ad14a25-4af5-47dd-9697-7f01d0ad8bcc">

## Nota máxima de los miembros del equipo

A fecha del 02/03/2024, todos los miembros del equipo, a saber;


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

han comunicado que desean optar a la máxima nota del proyecto, es decir, un 10.


## Formatos acordados en los repositorios de equipo

Se ha acordado seguir una política de [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/), en todos los repositorios del equipo. Además se seguirá una política en las ramas y pull requests que seguirán el siguiente formato:

`^(feature|bugfix|hotfix|chore|release)\/\d+-[\w-]+$`

Se establece, de común acuerdo entre el Project Manager (PM) y los Team Leads, que aquellos miembros del equipo que infrinjan estas políticas recibirán una primera advertencia, seguida de la posibilidad de recibir un 'strike' en caso de reincidencia.


## Responsabilidades individuales en S1

Se acuerda, mediante consenso, asignar responsabilidades individuales y compartidas a todos los miembros del equipo durante el Sprint 1. Es de suma importancia que estas tareas se completen dentro del plazo establecido, siendo acompañadas de posibles recompensas por su ejecución exitosa o, en caso de incumplimiento, de las consecuencias definidas en el Commitment Agreement. A continuación se describen las responsabilidades individuales comprometidas por cada miembro del equipo:


* AURORA NAVAS JIMÉNEZ
    * Gestión de usuarios pilotos
    * Governify
    * Esquema DB
    * Modelo DB
    * Despliegue
* CLAUDIA GILABERT PRIETO
    * Liderar el equipo de frontend
    * Estilos de la app
    * Exportar Mock-ups
    * Página de inicio
    * Despliegue
    * Conexión con el backend
    * Reunión con la ONG
    * Planificación del S2
* FÉLIX ÁNGEL GUDIEL GÜEMES
    * Problemas sucedido durante el S1
    * Reporte de IA
    * Populate
    * Upload documents to the DB
* FRANCISCO DE ASÍS ROSSO RAMÍREZ
    * Actividades de la NavBar
    * Login en NavBar
    * Clase de la NavBar
* FRANCISCO JAVIER CALDERÓN RODRÍGUEZ
    * Landing page
    * Pantalla de administración de socios
    * Pantalla de administración de cuenta
* IVÁN RAMÍREZ LARA
    * Pantalla de administración de socios
    * Pantalla de administración de cuenta
    * Dropdown de asociación
* MANUEL ORTIZ BLANCO
    * Análisis de costes
    * Arquitectura
    * Esquema DB
    * CRUD de Usuarios, Educadores, Socios, Voluntarios y Familias
* JUAN LUIS RUANO MURIEDAS
    * Estimaciones de ingresos
    * Populate
    * Esquema DB
    * Roles de usuario
    * CRUD de evaluación
* MANUEL FRANCISCO BARCIA JIMENEZ
    * Dropdown de la Homepage sobre la Asociación
    * Pantalla de Administrador de clases, eventos y proyectos
    * Análisis de costes
    * Arquitectura
* MARÍA NÚÑEZ REYES
    * Governify
    * Usuarios pilotos
    * Administración de familiares
    * Agenda 2030
* MARTA INÉS GONZÁLEZ DIÁNEZ
    * Retrospectiva
    * Presentación W4 y W5
    * Modificación de requisitos
    * Estilos de la app
    * Exportar Mock-ups
    * Información requerida por la ONG
    * Reunión con la ONG
    * Pantalla de Transparencia de la Homepage
* MIGUEL ANGEL ROMALDE DORADO
    * Liderar todo el proyecto
    * Github Actions
    * Análisis de costes
    * TCO: Capex, Opex
    * Modelo relacional
    * Creación de roles de usuario
    * CRUD de Usuarios, Educadores, Socios, Voluntarios y Familias
* PABLO PERIÁÑEZ CABRERO
    * Liderar el equipo de backend
    * Apéndice al agreement
    * Medidas de rendimiento
    * Autoevaluación/Rúbrica del S1
    * Cambio de DB a PostgreSQL
    * Modelo relacional
    * Planificación del S2
    * CRUD de Estudiantes y Autorizaciones de salida
    * Reunión con la ONG
* PEDRO LOPEZ RUZ
    * Arquitectura
    * Implementación del modelo de la DB
    * Creación de los roles de usuario
    * CRUD de Clases
* SAMUEL LUIS RODRÍGUEZ MANESS
    * Pantalla de formulario
    * Registro en la NavBar
* SERGIO AGUAYO OROZCO
    * CRUD de evento
    * CRUD de asamblea
    * Planificación del modelo
    * CRUD de donaciones
    * Revisitar CRUD de evento y crear CRUD de excursión

Cabe destacar que esto es una asignación de responsabilidades y no tiene relación con las actividades finalmente realizadas por cada miembro.

## Rendimiento del S2

Según las medidas explicadas anteriormente, los miembros del equipo han obtenido la siguiente evaluación según el rendimiento durante el Sprint2:

<img src="https://raw.githubusercontent.com/ISPP-G5/NexONG/main/Sprint2/Images/image.png" alt="PM"/>
<img src="https://raw.githubusercontent.com/ISPP-G5/NexONG/main/Sprint2/Images/image2.png" alt="TL_Back"/>
<img src="https://raw.githubusercontent.com/ISPP-G5/NexONG/main/Sprint2/Images/image3.png" alt="TL_Front"/>

## Responsabilidades individuales en S2

Se acuerda, mediante consenso, asignar responsabilidades individuales y compartidas a todos los miembros del equipo durante el Sprint 2. Es de suma importancia que estas tareas se completen dentro del plazo establecido, siendo acompañadas de posibles recompensas por su ejecución exitosa o, en caso de incumplimiento, de las consecuencias definidas en el Commitment Agreement. A continuación se describen las responsabilidades individuales comprometidas por cada miembro del equipo:

* AURORA NAVAS JIMÉNEZ
    * Deploy
    * Suggestion Model and CRUD
    * Pilots users management
    * Act as pilot user
    * Performance evaluation
    * Software review guidlines
* CLAUDIA GILABERT PRIETO
    * Frontend team lead
    * Frontend login
    * Favicon
    * Educators component
    * Kids evaluation
    * Deploy frontend
    * Partners
    * Educator evaluation
    * Act as pilot user
* FÉLIX ÁNGEL GUDIEL GÜEMES
    * AI Report
    * Business logic
    * Populate
    * Deploy
    * Act as pilot user
* FRANCISCO DE ASÍS ROSSO RAMÍREZ
    * Legal impact
    * Donations and Suggestions in navbar
    * Suggestion admin
* FRANCISCO JAVIER CALDERÓN RODRÍGUEZ
    * Landing page
    * Admin profile
    * Volunteer profile
    * Update profile
    * Act as pilot user
* IVÁN RAMÍREZ LARA
    * Volunteer, educators and partner admin
    * Add educator
    * Volunteer form
* MANUEL ORTIZ BLANCO
    * Poker planning
    * Expected aspects review
    * Failure Conditions review and check
    * AI Report
    * Backend documentation
    * Email validation
* JUAN LUIS RUANO MURIEDAS
    * Fixes for frontend
    * Authorisations for admin, educative centre, educator, volunteer, partner, student, family and volunteer
    * Act as pilot user
* MANUEL FRANCISCO BARCIA JIMENEZ
    * Customer agreement
    * Volunteer component
    * Volunteer agreement
    * Volunteer agenda
    * Volunteer attendance
    * Volunteer event
* MARÍA NÚÑEZ REYES
    * Problems encountered
    * Agreement with pilots users
* MARTA INÉS GONZÁLEZ DIÁNEZ
    * Manage the project as PM
    * Retrospective
    * Presentations
    * Storyboard
    * Evaluation and performance system
    * Frontend agenda
    * Act as pilot user
* MIGUEL ANGEL ROMALDE DORADO
    * TCO
    * Export the donations and punctual donations
    * Punctual donations CRUD
    * Payment method (Can be delayed to S3)
* PABLO PERIÁÑEZ CABRERO
    * Backend team lead
    * New evaluation and performace system
    * Poker planning
    * Commitment agreement
    * Expected aspect review
    * Documents name
    * Files organisation
* PEDRO LOPEZ RUZ
    * Learned lessons
    * RACI Matrix
    * FC teams review
    * Group organisation
    * Problems encountered
    * Backend documentation
    * Export Students
* SAMUEL LUIS RODRÍGUEZ MANESS
    * Problems encountered
    * Learned lessons
    * Demo video S2
    * Admin classes,projects and events
    * Activities educators
    * Event creation
    * Act as pilot user
* SERGIO AGUAYO OROZCO
    * Common database
    * Act as pilot user
    * Advertisement
    * Register and login
    * Authorisation framework


## Rendimiento del S3

Según las medidas explicadas anteriormente, los miembros del equipo han obtenido la siguiente evaluación según el rendimiento durante el Sprint3:

![image](https://github.com/ISPP-G5/NexONG/assets/72883992/f9392867-dea2-486c-bf4f-9d2d4fe17521)
![image](https://github.com/ISPP-G5/NexONG/assets/72883992/ee05e44e-99a7-44a1-8ffe-3f6135b6b4ef)
![image](https://github.com/ISPP-G5/NexONG/assets/72883992/e55b5118-0875-43be-9a9b-164a5a06a04e)

## Responsabilidades individuales en S3

Se acuerda, mediante consenso, asignar responsabilidades individuales y compartidas a todos los miembros del equipo durante el Sprint 3. Es de suma importancia que estas tareas se completen dentro del plazo establecido, siendo acompañadas de posibles recompensas por su ejecución exitosa o, en caso de incumplimiento, de las consecuencias definidas en el Commitment Agreement. A continuación se describen las responsabilidades individuales comprometidas por cada miembro del equipo:

* AURORA NAVAS JIMÉNEZ
    * Deploy
    * Comittement agreement with pilots users
    * Pilots users docs
    * Software Reviewer guidelines
    * Pilots users feedback
    * Google Compute engine
* CLAUDIA GILABERT PRIETO
    * Frontend team lead
    * Learned lessons
    * Token session
    * Donations export
    * Privacy policy
    * La Salle Homepage
    * Pilots users feedback
    * Deploy*
* FÉLIX ÁNGEL GUDIEL GÜEMES
    * TCO
    * Deployed software review*
    * Family authorizations
    * Evaluation
* FRANCISCO DE ASÍS ROSSO RAMÍREZ
    * Changelog
    * Recurring donations
    * Mission and values
    * Association information
    * Punctual donations
* FRANCISCO JAVIER CALDERÓN RODRÍGUEZ
    * Family registration
* IVÁN RAMÍREZ LARA
    * Summer School
    * Admin family request
    * Edit educator and volunteer
* MANUEL ORTIZ BLANCO
    * AI Report
    * Poker planning
    * Fix models and emails
    * Terms and conditions
* JUAN LUIS RUANO MURIEDAS
    * SLA
    * Script to deploy
    * Educator's tests
* MANUEL FRANCISCO BARCIA JIMENEZ
    * Customer agreement
    * Volunteer's calendar
    * Family's calendar
    * Volunteer attendance
* MARÍA NÚÑEZ REYES
    * Comittement agreement with pilots users
    * FC terms review
    * Pilots users
    * Volunteer document and formation
* MARTA INÉS GONZÁLEZ DIÁNEZ
    * Project manager leading
    * Commitment agreement
    * Presentation
    * Retrospective
    * AD
    * Marketing plan
    * Deploy
* MIGUEL ANGEL ROMALDE DORADO
    * Problems doc
    * Tests for partner and volunteer
    * Bug log
* PABLO PERIÁÑEZ CABRERO
    * Backend team lead
    * Commitment agreement
    * Poker planing
    * AD
    * Performance metrics
    * Time-effort report
    * Deploy
    * Load tests
* PEDRO LOPEZ RUZ
    * Problems doc
    * Learned lessons
    * Tests for admin, student & family
* SAMUEL LUIS RODRÍGUEZ MANESS
    * Demo S3
    * Info main page
    * Schedule for lessons
    * Partners membership
    * Lesson events
* SERGIO AGUAYO OROZCO
    * Common DB
    * Social login
    * Family kids
 
## Rendimiento del PPL

Según las medidas explicadas anteriormente, los miembros del equipo han obtenido la siguiente evaluación según el rendimiento durante el PPL:

![image](https://github.com/ISPP-G5/NexONG/assets/72883992/472b10df-06d9-4000-8d2d-e8a0706df188)
![image](https://github.com/ISPP-G5/NexONG/assets/72883992/3d5ef121-3600-4303-a03a-501b6524144f)
![image](https://github.com/ISPP-G5/NexONG/assets/72883992/955027bf-6dcc-421b-99a3-dd2b86d53b74)


## Responsabilidades individuales en PPL

Se acuerda, mediante consenso, asignar responsabilidades individuales y compartidas a todos los miembros del equipo durante el PPL. Es de suma importancia que estas tareas se completen dentro del plazo establecido, siendo acompañadas de posibles recompensas por su ejecución exitosa o, en caso de incumplimiento, de las consecuencias definidas en el Commitment Agreement. A continuación se describen las responsabilidades individuales comprometidas por cada miembro del equipo:

* AURORA NAVAS JIMÉNEZ
    * Final Deploy
    * Fix model
    * Fix HTML payment
    * Deployed software review
* CLAUDIA GILABERT PRIETO
    * Frontend team lead
    * Fix evaluation educator
    * Final release
    * Project summary docuementation
    * WPL Promotion
* FÉLIX ÁNGEL GUDIEL GÜEMES
    * Pilot user
    * UX Report
    * Fix family evaluation
* FRANCISCO DE ASÍS ROSSO RAMÍREZ
    * Organisation feature
    * Sugestion emails
    * Changelog
    * Pilot user
    * Business plan
* FRANCISCO JAVIER CALDERÓN RODRÍGUEZ
    * Confirmation message
    * Partner profile
    * Marketing plan
    * Social media posts
* IVÁN RAMÍREZ LARA
    * Fix meetings
    * Pilot user
    * Marketing plan
    * Social media posts
* MANUEL ORTIZ BLANCO
    * Fix activation page
    * AI Usage
    * Poker planing
* JUAN LUIS RUANO MURIEDAS
    * Fix donation
    * Learned lessons
    * Business plan
* MANUEL FRANCISCO BARCIA JIMENEZ
    * Volunteer attendance
    * Volunteer's calendar
    * Marketing plan
    * Social media posts
* MARÍA NÚÑEZ REYES
    * Pilots user
    * Volunteer formation
    * Style and toast
* MARTA INÉS GONZÁLEZ DIÁNEZ
    * Project manager leading
    * Investors ad
    * Presentations
    * Retrospective
    * Improve ad v2
    * Improve investors ad
* MIGUEL ANGEL ROMALDE DORADO
    * TCO
    * Learned lessons
    * FC terms review
* PABLO PERIÁÑEZ CABRERO
    * Backend team lead
    * Commitment agreement apendix
    * Performance evaluations
    * Group evaluations
    * Poker planning
    * Project summary docuementation
    * Time effort report
    * Fix volunteer model
* PEDRO LOPEZ RUZ
    * Pilot user
    * Problems document
* SAMUEL LUIS RODRÍGUEZ MANESS
    * Demo PPL
    * Partner membership
    * Fix admin lesson
* SERGIO AGUAYO OROZCO
    * Fix family
    * Fix students time out
    * Landing page
    * Common database
    * FC terms review
