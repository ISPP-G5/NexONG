# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp; 5-Project-Documentation-Backend - PPL
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

<a name="br2"></a> 

## Índice
1. Introducción
2. Trabajo realizado
3. Trabajo futuro
4. Trabajo por mejorar

## Registro de cambios
**Versión** | **Fecha** | **Descripción**| **Redacción** | **Revisión**
--- | --- | --- | --- | --- 
1.0.0 | 29/4/2024 | Semana 12 |Pablo Periañez Cabrero| Aurora Navas Jiménez


## Introducción
El objetivo principal de este documento es la creación de una guía que contenga información sobre las tareas que se han realizado durante el desarrollo del proyecto, que tareas han quedado pendiente y que se podrían implementar en el futuro, así como que partes de las ya implementadas podrían ser mejoradas para así hacerlas más eficientes y ajustarnos de mejor manera a los requisitos dados por la ONG Manos Abiertas con Norte, nuestro actual cliente.

este documento incluye la parte que corresponde al backend. Por lo tanto, lo relativo al frontend se ha mantenido en otro documento separado para facilitar su lectura.
## Organización del repositorio
En el caso de nuestro grupo NexONG se acordó la creación de una organización en la que se crearían diferentes repositorios: uno para la documentación, otro para la landing page, otro para el Backend y finalmente uno para el Frontend.

Al tener diferentes repositorios de trabajo, a nosotros personalmente nos facilitó el trabajo ya que nos permite localizar la información que queremos de manera rápida, en cambio si todo estuviera en un mismo repositorio sería más complicado. 

En el repositorio del Backend se ha seguido el flujo de trabajo de GitFlow dónde la rama Develop es en la que se ha ido desarrollando, se ha creado una rama Deploy para el despliegue que siguiendo la estructura de GitFlow es la rama de publicación. Además, el contenido de Develop se pasa a Main para realizar un release con su correspondiente etiqueta.

A la hora del desarrollo se utilizó el apartado de issues para describir que tareas hay que realizar si son features o fixes (estas son las dos principales que hemos tenido) así como los issues relacionados con el release y despliegue.

Cada issue estaba asignado a una o dos personas como mucho con su etiqueta correspondiente, deadline y proyecto. Cada issue completado es seguido por su correspondiente pull request donde tenemos un workflow de Codacy y la GitHub action de Black_Formatter para asegurar que se cumple la calidad y el estilo de código. Cada pull request es revisada por tres personas, siendo siempre uno de ellos el Team Leader del Backend para garantizar que el trabajo realizado cumple con lo esperado. 

El Team Leader, era también el que creaba y asignaba los issues a cada persona de su grupo. Esta organización, creación y asignación de tareas era consultada entre PM y el team leader del backend para que se supiera en todo momento en que se iba a trabajar y si lo que se quería realizar por parte del Backend es posible (teniendo en cuenta que la parte correspondiente del Backend estuviera creada). 

Como se ha indicado se han utilizado los proyectos de GitHub ya que facilita la organización de los repositorios y sus tareas gracias al tablero Kanban que ofrece que permite visualizar la tarea,  el/la asignado/a, el deadline y los revisores. Los revisores también eran establecidos por los Teams Leader en su correspondiente repositorio para así garantizar que todos los miembros revisaran código de sus compañeros.

## Trabajo realizado
Una vez recopilados los requisitos de parte de nuestro cliente, se analizaron y estudiaron para poder así entender de manera más profunda que es lo que necesitaban y esperaban del software que se iba a desarrollar. 

Una vez con toda esa información en mente, se crearon los diagramas conceptuales de la base de datos, una vez que se decidió el uso de PostgreSQL y Django.

Con toda la información precedente de los requisitos, así como el diagrama, se realizó una primera planificación de las tareas a realizar que por cuestiones del tiempo disponible, así como organización del equipo se vio la necesidad de reducir el alcance y de realizar una re-planificación. Toda esta documentación puede encontrarse en la carpeta de #DP. También puede ser de gran utilidad el documento que se elaboró para la planificación de backend llamado "Requisitos".

## Trabajo pendiente por realizar
Manos Abiertas ampliaba mucho el alcance en cada reunión que teníamos, es por ello por lo que tuvimos que recortar funciones que para ellos serían esenciales. A partir de aquí se discutirán las tareas que fueron imposible realizar debido al corto alcance del proyecto.

- En general el backend está bastante implementado y completo, pero en cierto punto se dejaron de tener en cuenta las nuevas features del backend en el desarrollo del frontend por el hecho de recortar alcance.

- Un nuevo tipo de usuario, dedicado al centro educativo: Este usuario podrá dar de alta a alumnos de mañana en el sistema, notificando a la ONG y a la familia. Y sin necesidad de usar tanto papelo y sobrecarga a la ONG. Al principio se tuvo en cuenta y se avanzó en esta feature, pero llegado a un punto se recortó el alcance y no se llegó a implementar.

- Más flexibilidad en los eventos.

- Notificaciones por correo de lo que está sucediendo en la ONG.

- Mensajería dentro de la propia aplicación. Evitando usar y saturar el teléfono y Whatsapp de la ONG.

- Implementación del apartado de proyecto de la ONG: Donde puedan llevar un seguimiento de los proyectos y su financiación de la ONG. Al final es como la ONG basa su funcionamiento.

- Gestión dinámica de la página web: Proporcionar al administrador recursos para modificar la página web principal sin tener que programar en React. Los datos deberían de guardarse en el backend y mostrarse en la web principal, siendo modificable fácilmente por el administrador, sin que tenga conocimientos técnicos (Estilo Wordpress).
  
- El frontend debería de incluir todas las exportaciones que se hizo en el backend para sacar los datos de la base de datos a formato CSV, PDF y Excel. Y actualmente no se está usando.


## Cosas para mejorar
Dejando a un lado nuevas funcionalidades, existen funcionalidad que están implementadas, pero se deberían de mejorar y optimizar.

- El más claro, es el modelo conceptual de la base de datos. Ya que lo que empezó siendo una cosa simple y se le fueron añadiendo tablas y relaciones. El resultado fue un modelo bastante ineficiente ya que el frontend depende de varias consultas para averiguar datos de las personas debido a relaciones 1:1.
  
- Puede ser una opción, que se planteó desde el principio, pero debido a que muchos no tenían experiencia, no fue posible implantarlo. Es el hecho de usar una base de datos NoSQL. Éstas pueden ser más eficiente y más flexibles a la hora de tener muchos roles y usuarios distintos, ya que la base de datos es mucho más adaptable. Además, empresas como MongoDB, ofrecen bases de datos desplegadas en la nube (MongoDB Atlas) gratis. Actualmente se usa PostgreSQL y cuesta 3-4$ al día.

## Conclusión
Se ha desarrollado una pequeña guía con la información correspondiente que se ha realizado durante el proyecto, así como las cosas que se pueden mejorar y las cosas que no han sido posible implementar. Este proyecto ha supuesto una gran carga de trabajo, debido a eso y a que ISPP es una asignatura de 6 ECTS no se ha podido completar todo como nos hubiera gustado. Sin embargo, se ha obtenido un buen resultado, en el que todos hemos colaborado lo mejor que hemos podido.

