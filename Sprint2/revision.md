# Software Review Guidelines - Sprint 2
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
1. Mapeo de los usos core
2. Información necesaria para la prueba

## Registro de cambios
| Versión | Fecha | Descripción | Redacción | Revisión |
|---------|-------|-------------|---------------|-|
|1.0.0|30/03/2024|Sprint 2 guidelines|AURORA NAVAS JIMÉNEZ|PABLO PERIÁÑEZ CABRERO|

## 1. Mapeo de los usos core
En nuestro caso, los usos core han cambiado un par de veces a lo largo del proyecto. Esto se debe a que en cada reunión con Manos Abiertas con Norte los requisitos se refinaban un poco más, con lo cual, no tiene ningún sentido que los casos de uso core iniciales persistieran. Finalmente, estos son nuestros casos de uso core:

### Sprint 2
- **Panel de administrador**
	- *Administración de voluntarios:* deben hacer operaciones RUD con voluntarios. En la app desplegada el administrador puede ver a los voluntarios, eliminarlos y ver/aceptar/rechazar solicitudes. .
	- *Administración de educadores:* deben hacer operaciones CRUD con educadores. En la app desplegada el administrador puede verlos y eliminarlos.
	- *Administración de socios*: deben hacer operaciones RUD con socios y hacer operaciones CRUD con asambleas. En la app desplegada el administrador puede verlos, eliminarlos y convocar asambleas. 
	- *Administración de familias:* deben hacer operaciones RUD con las familias y aceptar/denegar solicitudes de éstas. En la app desplegada, esto no está implementado.
	- *Administración de clases:* deben hacer operaciones CRUD con clases.  En la app desplegada el administrador puede hacer operaciones CED.
	- *Administración de eventos:* deben poder hacer operaciones CRUD con eventos. En la app desplegada el administrador puede hacer las operaciones CRUD correspondientes.
	- *Administración de sugerencias:* deben poder hacer operaciones RD con sugerencias. En la app desplegada el administrador puede verlas.
- **Página home:** diferentes ventanas navegables en las que la ONG puede anunciar su labor. Está en la app desplegada.
- **Página de voluntarios:** los voluntarios podrán ver los eventos y las clases, a los cuales se podrán apuntar y/o editar o borrar su asistencia. En la app desplegada, los voluntarios pueden ver los eventos disponibles y apuntarse a ellos.
- **Página de educadores:** los educadores podrán ver sus clases y a sus alumnos. Además, podrán evaluarles. En la app desplegada, esto no está implementado.
- **Página de familias:** las familias podrán hacer operaciones CRUD con sus hijos y ver las evaluaciones de los educadores. En la app desplegada, esto no está implementado.
- **Página de socios:** los socios podrán hacer operaciones CRU con sus donaciones. En la app desplegada, esto no está implementado.
- **Página de centros educativos:** los centros educativos podrán hacer operaciones CRUD con sus estudiantes y ver las evaluaciones de los educadores. En la app desplegada, esto no está implementado. Aclaración: en Manos Abiertas con Norte hay dos tipos de estudiantes: de tarde y de mañana. Los de mañana son alumnos expulsados de sus centros y la ONG tiene la obligación de darles clase durante la mañana. Además, son responsables por ellos lo propios centros educativos. Los estudiantes de tarde son aquellos que sus familias apuntan. La ONG debe aceptarlos o rechazarlos.
> [!NOTE] 
> Cabe destacar que todos los usos core, además de la autenticación, están realizados en la API, pero no en el frontend.

## Información necesaria para la prueba
### Sprint 2
#### Pantallas a probar (incluyendo credenciales)
- La URL del **despliegue del frontend** es [esta](https://nexong.ew.r.appspot.com/).
- La URL del **despligue del backend** es [esta](https://nexongapi.ew.r.appspot.com/api/). Además, puede ver su documentación en Swagger [aquí](https://nexongapi.ew.r.appspot.com/docs/).

_Página de Inicio_
- Pueden navegar a través de las diferentes pantallas. Tengan en cuenta que nada del registro está completado aún.
- Sabemos que las páginas "La Salle" y "Organización" están vacías.
- En "Transparencia", la descarga de archivos no funciona aún.
- Pueden hacer donaciones puntuales y sugerencias.

_Panel de administrador_
- Inicie sesión con el usuario admin@gmail.com y contraseña *admin*.
- Voluntarios; pueden verlos, borrarlos y ver/aceptar/rechazar las solicitudes de los voluntarios. Queremos que en un futuro al darle a "Descargar" se descargue en un archivo zip toda la documentación entregada por el voluntario. **Por favor, no borren a el voluntario llamado Marco Castilla.**
- Educadores; pueden verlos y borrarlos. En un futuro el administrador también los creará, ya que los educadores no se registran en la página.
- Socios; pueden verlos, borrarlos y convocar una asamblea. **Por favor, no borren al socio llamado Esteban Rodriguez.**
- Eventos; pueden verlos, crearlos, borrarlos y editarlos.
- Sugerencias; pueden verlas.

_Voluntarios_
- Inicie sesión con el usuario mcast@gmail.com y la contraseña *volutalio1*.
- Puede ver y apuntarse a eventos.

_Socios_
- Inicie sesión con el usuario esteban@gmail.com y la contraseña *parnerio1*.

#### Otras URL solicitadas

|                  | URL | Observations |
|------------------|-----|-|
| Landing page     |https://ispp-g5.github.io/| | 
| GH backend       |https://github.com/ISPP-G5/NexONG_Backend|The deployment code is in branch *deploy/s2*|
| GH frontend      |https://github.com/ISPP-G5/NexONG_Frontend|              |
| GH documentation |https://github.com/ISPP-G5/NexONG|              |
| Clockify         |[https://app.clockify.me/shared/66085b400f0fa031f07dd478](https://app.clockify.me/shared/660996276cf4e742fab78a5b)|              |
| Demo video       | |The demo video is on the last release of the documentation repository|
