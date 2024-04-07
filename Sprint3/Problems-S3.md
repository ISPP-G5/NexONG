# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Problemas - Sprint 3
# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NexOng - Grupo 5


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
1. Registro de cambios
2. Introducción
3. Registro
4. Soluciones

## Registro de cambios
**Versión** | **Fecha** | **Descripción**| **Redacción** | **Revisión**
--- | --- | --- | --- | --- 
1.0.0 | 7/3/2024 | Semana 6 | SAMUEL LUIS RODRÍGUEZ MANESS | MARÍA NÚÑEZ REYES
2.0.0 | 16/3/2024 | Semana 7 | MARÍA NÚÑEZ REYES | CLAUDIA GILABERT PRIETO
3.0.0 | 30/3/2024 | Semana 8 | PEDRO LÓPEZ RUZ | SAMUEL LUIS RODRÍGUEZ MANESS
4.0.0 | 7/4/2024 | Semana 9 | PEDRO LÓPEZ RUZ Y SAMUEL LUIS RODRÍGUEZ MANESS | MARÍA NÚÑEZ REYES



## Introducción
Este documento recopila los problemas encontrados a lo largo de todo el proceso de desarrollo del proyecto. Por cada problema se especifica el conflicto en sí, cuando se dio, cómo (y cuándo) se resolvió y el impacto que tuvo sobre el proyecto.

Este historial no debe sólo informar sobre el historial del desarrollo de la aplicación, si no también servir como referencia para futuros problemas y poder actuar en concordancia a ellos.

## Registro
### Desacuerdos y falta de confianza entre miembros del equipo
Algunos miembros del equipo han mostrado su frustración en la reunión del día 5 de marzo ante la actitud que se ha presentado a la hora de comunicarse con sus líderes o con otros compañeros. Se han detectado faltas de respeto y de orden por lo que se ha hecho uso de una mediadora para resolver este problema.

### Disconformidad general con las medidas de auto evaluación del equipo y falta de transparencia
La mayoría del equipo ha sentido que las medidas de evaluación que se realizan sobre otros miembros no han sido correctas. Por una parte, es complicado ofrecer una valoración realista a las personas con las que menos contacto se ha tenido, además no se ha considerado algunas valoraciones justas cuando algunas encuestas son de carácter objetivo. Luego, se desea buscar un nivel más alto de transparencia a la hora de realizar la rúbrica del rendimiento de cada persona, para poder presentar dudas y tener los motivos de nuestra nota visibles.
En la reunión del pasado marte 12 de marzo, se ha seguido mostrando disconformidad con las notas anteriores. Parte del equipo ha sentido que las medidas de evaluación que se realizan sobre otros miembros no han sido correctas ni justas. Por una parte, es complicado ofrecer una valoración realista a las personas con las que menos contacto se ha tenido, además no se ha considerado algunas valoraciones justas cuando algunas encuestas son de carácter objetivo. Luego, se desea buscar un nivel más alto de transparencia a la hora de realizar la rúbrica del rendimiento de cada persona, para poder presentar dudas y tener los motivos de nuestra nota visibles.

### Problemas con las políticas de ramas y commits
Las políticas de ramas y de commits buscan asegurar el cumplimiento uniforme y correcto al trabajar con git flow, pero se ha comprobado que también puede causar problemas. Algunos conflictos de una rama por las medidas del conventional commits acabaron afectando a varios miembros de modo que no podían hacer sus Pull Requests.

### Miembros desconocen el estado general del proyecto
Algunos miembros del equipo no realizan sus tareas de forma correcta y hay pérdidas de tiempo al no leer todos los requisitos del cliente y no dedicar un repaso al estado del progreso del proyecto, y lo que están haciendo otros miembros. Esto también provoca tener que empezar algunas tareas desde el principio.

### Poca atención a la descripción de las issues por parte de algunos miembros
Algunos miembros del equipo han visto retrasos en sus tareas por no comprender los requerimientos de algunas issues por no leer detenidamente la descripción de éstas.

### Discordancia entre backend y frontend
La coordinación entre backend y frontend no ha sido muy acertada esta semana. Debido a la incompatibilidad de los atributos necesitados en frontend y los implementados en backend, el equipo de frontend ha tenido que aplazar alguna issue y adelantar contenido del sprint 3 para tener suficiente trabajo que implementar esta semana. Esto puede haberse debido a la disparidad en la planificación inicial, errores de concepción de algunos requisitos y falta de seguimiento del *mockup*.

### Merge Problemático

Un miembro del equipo al integrar una funcionalidad realizó por error un pull de una rama que no debería haber hecho provocando fallas en las siguientes implementaciones a partir de esa.

### Incumplimiento Commitment Agreement por los usuarios pilotos

El grupo de la tarde y el nuetro firmamos un commitment agreement en el cual nos comprometiamos a desplegar la aplicación el lunes 25 de marzo  y tener para testear ese mismo lunes hasta el miercoles 27 de marzo. Llegado ese lunes nuestro grupo ya tenía desplegado la aplicación como habíamos firmado, pero el otro grupo no estaba en la misma situación alegando a una miembro de nuestro equipo que habian tenido problemas y que si podíamos cambiar el commitment agreement a más tarde, a lo que nosotros respondimos con una negativa debido a que ya estaba firmado y cambiarlo supondría el imcumplimiento total del mismo.

### Problemas con los permisos de algunas funcionalidades

Durante la realización de los test en el backend, varios compañeros se dieron cuenta de que faltaban permisos para una serie de funcionalidades como por ejemplo la creación de familias. Tras investigar la causa se comprobó que provenía de una implentación, la cual, trataba de adjuntar los permisos admin de las aplicaciones, pero durante el desarrollo de la misma omitió algunos permisos provocando errores. Debido a esto el frontend no pudo trabajar de manera fluida debido que se les impedían realizar varias funciones para probar sus métodos implemetados.

Haciendo enfoque en la parte del frontend, por errores similares al mencionado anteriormente algunos miembros han tenido que empezar sus tareas más tarde de lo habitual y han sido acabadas mucho más cerca de la deadline, mientras que otras no han sido terminadas.

 

## Soluciones
Las soluciones que se pondrán o ya se han puesto en marcha para resolver los problemas anteriores son los siguientes:
- Mediante un mediador, se ha recordado a las personas involucradas en el conflicto personal lo importante que es el respeto entre los miembros de un equipo y se ha llegado a un compromiso mediante el diálogo para continuar el proyecto lo mejor posible.
- Se ha creado un nuevo sistema de evaluación entre los miembros del equipo que ha sido votado por los miembros. Queda por aprobarse para que se convierta en el modelo de evaluación oficial. Algunas de estos cambios son:
   - Baja el porcentaje a 10%
   - Se simplifica la rúbrica, eliminando algunos apartados objetivos
   - Se incluye el poker planning como medida objetiva para el rendimiento
   - Los miembros del equipo miden el rendimiento del PM y los Team Leader
- Se han relajado las restricciones a la hora de hacer commits para evitar posibles desastres por bloqueos. Sin embargo, el incumplimiento continuo de las conventional commits se penalizará tras varios avisos.
- Se le recordará a los miembros del equipo la importancia de hacer una revisión general al proyecto, de informarse sobre los requerimientos de su tarea y de leer bien las descripciones de las issues. También hay que esforzarse por escribir descripciones lo más claras y detalladas posibles, así como dejar un buen comentario de revisión.
- Buscar una mayor alineación entre los requerimientos solicitados por las páginas y la base de datos del backend a través del diálogo entre ambos equipos.
- Una vez se localizó el problema del merge se creo un rama Hotfix para intentar mitigar los daños causados 
- Tras trasladar nuestro pensamiento de no cambiar el commitment agreement, los usuarios piloto del grupo de tarde aceptaron las condiciones a muy a su pesar y enviaron una versión desplegada de la apliación ese mismo día.



- Tras localizar los errores se lanzó una rama hotfix que corregía dichos permisos y se lanzó una pull request para comprobar que verdaderamente se había realizado el cambio.
- Se notificó a los miembros de frontend del arreglo y se consiguió trabajar en condiciones finalmente.

## Resultados

Los resultados tras la aplicación de las soluciones

- Tras la mediación se ha obtenido un ambiente de trabajo más calmado, en donde se realizan comentarios por cada discrepacia que vaya apareciendo para llegar a un concenso entre todos los miembros del grupo.
  
- Respecto al sistema de evaluaciación a día de la realización del documento se desconoce cual será la complicidad del equipo una vez conozcan los resultados.
  
- Tras relajar las restricciones a la hora de realizar los commits y pull request ha fluido un poco mejor el trabajo pero todavia a final de semana seguian habiendo pull requests por aprobar y por ello se ha sugerido que todos los miembros del equipo activen las notificaciones por email para mitigar la ralentización.
  
- Una vez dejado claro la importancia de realizar una buena lectura de las issues y esforzarse por escribir descripciones lo más claras y detalladas posibles, así como dejar un buen comentario de revisión, han aparecido nuevos comentarios en las reviews mucho más ricas tanto por parte de quien ha implementado la issue incorporando formas de como acceder a la tarea realizada y como probarla, tanto por parte de los revisores.
  
- Acerca de la comunicación entre backend y fronted, se ha incrementado la participación de los miembros de frontend preguntando dudas al equipo de backend, aunque todavía hay discrepacias lingüisticas entre miembros, es por ello que varias personas en la retrospectiva han propuesto realizar una reunión en próximas semana entre ambos equipos.
  
- Tras revertir los cambios, el miembro del equipo en cuestión pidió perdón y revirtió el merge en su rama haciendo que se solucionase el problema. Además al integrarse la rama hotfix en develop, los demás miembros al hacer pull de la misma en sus ramas, solucionaron los errores causados.
  
- Cuando los usuarios pilotos de nuestro grupo accedieron a la versión desplegada del grupo de tarde, rápidamente se dieron cuenta de que era una versión bastante básica sin apenas funcionalidades, por lo que no pudieron testear demasiado.
  
- Una vez aceptada la pull request e integrada en la rama develop, el equipo frontend pudo trabajar sin ningun tipo de problema.


