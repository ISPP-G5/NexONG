# Software Reviewer Guideline - WPL
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
1. Sprint 2
	1. Mapeo de los usos core
	2. Información necesaria para la prueba
2. Sprint 3
	1. Mapeo de los usos core
	2. Información necesaria para la prueba
3. PPL
4. WPL
	1. Mapeo de los usos core
	2. Información necesaria para la prueba

## Registro de cambios
| Versión | Fecha | Descripción | Redacción | Revisión |
|---------|-------|-------------|---------------|-|
|1.0.0|30/03/2024|Sprint 2 guidelines|AURORA NAVAS JIMÉNEZ|PABLO PERIÁÑEZ CABRERO|
|2.0.0|19/04/2024|Sprint 3 guidelines|AURORA NAVAS JIMÉNEZ|FÉLIX ÁNGEL GUDIEL GÜEMES|
|2.0.1|22/04/2024|Adición de información tras revisión del revisor|AURORA NAVAS JIMÉNEZ|FÉLIX ÁNGEL GUDIEL GÜEMES|
|2.0.2|06/05/2024|Información del PPL|AURORA NAVAS JIMÉNEZ|PABLO PERIÁÑEZ CABRERO|
|3.0.0|19/05/2024|Información del WPL|AURORA NAVAS JIMÉNEZ|FÉLIX ÁNGEL GUDIEL GÜEMES|

## 1. Sprint 2
### 1.1 Mapeo de los usos core
En nuestro caso, los usos core han cambiado un par de veces a lo largo del proyecto. Esto se debe a que en cada reunión con Manos Abiertas con Norte los requisitos se refinaban un poco más, con lo cual, no tiene ningún sentido que los casos de uso core iniciales persistieran. Finalmente, estos son nuestros casos de uso core:
- **Panel de administrador**
	- *Administración de voluntarios:* deben hacer operaciones RUD con voluntarios. En la app desplegada el administrador puede ver a los voluntarios, eliminarlos y ver/aceptar/rechazar solicitudes.
	- *Administración de educadores:* deben hacer operaciones CRUD con educadores. En la app desplegada el administrador puede verlos y eliminarlos.
	- *Administración de socios*: deben hacer operaciones RUD con socios y hacer operaciones CRUD con asambleas. En la app desplegada el administrador puede verlos, eliminarlos y convocar asambleas. 
	- *Administración de familias:* deben hacer operaciones RUD con las familias y aceptar/denegar solicitudes de éstas. En la app desplegada, esto no está implementado.
	- *Administración de clases:* deben hacer operaciones CRUD con clases.  En la app desplegada el administrador puede hacer operaciones CED.
	- *Administración de eventos:* deben poder hacer operaciones CRUD con eventos. En la app desplegada el administrador puede hacer las operaciones CRUD correspondientes.
	- *Administración de sugerencias:* deben poder hacer operaciones RD con sugerencias. En la app desplegada el administrador puede verlas.
- **Página home:** diferentes ventanas navegables en las que la ONG puede anunciar su labor. Está en la app desplegada.
> [!NOTE] 
> Cabe destacar que todos los usos core están realizados en la API, pero no en el frontend. En el Sprint 3 se terminará la completa implementación de los casos de uso core además de la autenticación y el sandbox de pago.
### 1.2 Información necesaria para la prueba
#### Pantallas a probar (incluyendo credenciales)
- La URL del **despliegue del frontend** es [esta](https://nexong.ew.r.appspot.com/).
- La URL del **despligue del backend** es [esta](https://nexongapi.ew.r.appspot.com/api/). Además, puede ver su documentación en Swagger [aquí](https://nexongapi.ew.r.appspot.com/docs/).

>[!NOTE]
>Podría ocurrir que al entrar en alguno de los dos despliegues diera un `Server Error`. Esto se daría en caso de que los créditos se hubieran consumido. Estaremos atentos a que esto no pase, pero, si ocurriera, por favor avísennos.

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

## 2. Sprint 3
### 2.1 Mapeo de los usos core
Estos son nuestros casos de uso core:
- **Panel de administrador**
	- *Administración de voluntarios:* deben hacer operaciones RUD con voluntarios, además pueden aceptar o rechazar solicitudes, y descargar en un ZIP los documentos adjuntados en el proceso de registro por el voluntario.
	- *Administración de educadores:* deben hacer operaciones CRUD con educadores. 
	- *Administración de socios*: deben hacer operaciones RUD con socios y crear asambleas. Además, es posible descargar las donaciones en PDF, CSV o Excel.
	- *Administración de familias:* deben ver a las familias y a sus hijos y aceptar/denegar solicitudes de éstas. 
	- *Administración de clases:* deben hacer operaciones CRUD con clases.
	- *Administración de eventos:* deben poder hacer operaciones CRUD con eventos. La diferencia entre un evento y una actividad es que las actividades están asociadas a una clase.
	
- **Página home:** diferentes ventanas navegables en las que la ONG puede anunciar su labor. 
- **Operaciones no matchmaking:** 
	- *Registro:* en nuestra aplicación te puedes registrar como voluntario, familia o socio.
	- *Pago:* en la página de "Donaciones" cuando no se ha iniciado sesión, existen las **Donaciones puntuales**. Como tarjeta de prueba puede usar 4242 4242 4242 4242 como número de tarjeta, 12/29 como fecha de caducidad y 123 como CVC.
	- *Consumo:* iniciando sesión como cualquier tipo de usuario, se podrá consumir nuestro servicio. En la siguiente sección, se listarán todos los servicios que se pueden consumir y como hacerlo.

### 2.2 Información necesaria para la prueba
#### Pantallas a probar (incluyendo credenciales)
- La URL del **despliegue del frontend** es [esta](https://nexong-s3-1.oa.r.appspot.com/).
- La URL del **despligue del backend** es [esta](https://nexongapi-s3.ew.r.appspot.com/api). Además, puede ver su documentación en Swagger [aquí](https://nexongapi-s3.ew.r.appspot.com/docs).

>[!NOTE]
>Podría ocurrir que al entrar en alguno de los dos despliegues diera un `Server Error`. Esto se daría en caso de que los créditos se hubieran consumido. Estaremos atentos a que esto no pase, pero, si ocurriera, por favor avísennos.

**Página de Inicio**
- Pueden navegar a través de las diferentes pantallas.
- Pueden hacer donaciones puntuales y sugerencias.

**Panel de administrador**
Inicia sesión con las credenciales **info.nexong@gmail.com/m4n0s4bi3rt4sc0nn0rt3**.  
- _Perfil_: puedes ver el perfil de administrador y actualizarlo.  
- _Voluntarios_: puedes verlos, borrarlos y editarlos.
- _Voluntarios > Solicitudes_: puedes ver/aceptar/rechazar y descargar un zip con los documentos de las solicitudes de los voluntarios. 
- _Educadores_: puedes verlos, borrarlos y editarlos. 
- _Educadores > Añadir educador:_ puedes crear un educador.
- _Socios_: puedes verlos, borrarlos y editarlos. También, puedes descargar todos las donaciones en formato pdf, excel o csv y convocar una asamblea. 
- _Familias_: puedes ver las familias y la información de sus hijos  
- _Familias > Solicitudes_: puedes ver/aceptar/rechazar y descargar un documento pdf de las solicitudes de nuevos niños.  
- _Clases_: puedes verlas, editarlas y borrarlas. 
- _Clases > Crear clase_ : puedes crear una clase.
- _Clases > Crear horario_ : puedes crear un horario para la clase.
- _Eventos_: puedes verlos, crearlos, borrarlos y editarlos (si creas un evento haciendo click en el calendario, la fecha de inicio se pone automáticamente).  
- _Sugerencias:_ puedes verlas y borrarlas.  
- _Documentos_: aquí se suben los documento que aparecen en la página "Transparencias" de la página de inicio. Al añadir el documento, este se podrá ver en la tabla de la página mencionada y al hacer click se puede descargar este documento.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de voluntarios**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como voluntario" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**). Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta. Revise el Spam.
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro. 
-  _Formulario_: el usuario, al ser un nuevo voluntario, debe completar el formulario con la información. Los botones de descarga son los documentos que el usuario debe subir rellenados y firmados (excepto el de delitos sexuales que explica como conseguir ese documento). Si el voluntario es menor de edad, tendrá que subir dos documentos más (aparece automáticamente). **SOLO SUBIR ALGÚN ARCHIVO PDF, NO HACE FALTA SUBIR DICHOS DOCUMENTOS FIRMADOS.** La fecha de incorporación no es necesaria. Tras completarlo, una pantalla de espera aparecerá y el voluntario permanecerá ahí hasta que sea aceptado. Si es rechazado, el estado cambiará pero la página seguirá activa.  
- **CIERRE SESIÓN e inicie sesión como administrador con las credenciales anteriores**: En Voluntarios > Solicitudes, acepte la solicitud del voluntario creado. Aquí puedes descargar el zip con los documentos.  
- **CIERRE SESIÓN e inicie sesión con las credenciales del voluntario otra vez**: Ahora el voluntario puede ver su pantalla.

>[!WARNING]
>Respecto a las credenciales que se presentan a partir de aquí; hay que tener en cuenta que estos usuarios se han creado a partir de un `python manage.py loaddata populate.json`. Con lo cual, estos usuarios no contienen archivos reales y toda acción que manipule esos archivos pueden dar problemas. Por ello, recomendamos usar los usuarios recién creados.

**Panel de voluntarios**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **mcast@gmail.com/contraseña**.
- _Agenda_: Puede ver y apuntarse a eventos y a actividades.  
- _Asistencia_: Puede ver sus asistencias y borrarlas. 
-  _Perfil_: puede actualizar la información. También, **puede borrar los datos de la página web (derecho al olvido) lo cual necesitamos hacer para continuar testeando, ya que no podrá crear otra cuenta con el mismo correo**.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de familias**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como familiar" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).   
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro.

**Panel de familia**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **annanna@gmail.com/contraseña**.
- *Niños:* Puedes ver a tus hijos. Puedes registrar a hijos, que deberán ser aceptados/rechazados por el administrador, como los voluntarios.
- *Evaluación diaria:* Puedes ver las evaluaciones diarias de cada hijo. 
- *Evaluación anual:* Puedes ver las evaluaciones anuales de cada hijo. 
- *Autorizaciones:* Puedes subir las autorizaciones para eventos de cada hijo. Además de ver autorizaciones anteriores y ver actividades disponibles.
- *Calendario:* Puedes ver las clases, eventos y actividades de los hijos.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de socios**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como socio" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).   
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro.

**Panel de socio**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **esteban@gmail.com/contraseña**.
- *Calendario:* puede ver los eventos y las asambleas.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de educadores**
- Inicia sesión con la cuenta de administrador.
-  _Educadores > Añadir educador:_ puedes crear un educador, ya que los educadores no se registran en la página (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro. 

**Panel de educador**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **palomino@gmail.com/contraseña**.
- Puedes ver un listado de los niños asociados a clases asociadas con tu usuario de educador.
- Puedes ver los datos de contacto de los niños.
- Puedes poner un comentario en cada evaluación, sin embargo, aún no puedes poner nota.
- Puedes ver la asistencia de los alumnos a futuras actividades.
- Tras probar la funcionalidad completa, _Cierre Sesión_.

#### Otras URL solicitadas

|                  | URL | Observations |
|------------------|-----|-|
| Landing page     |https://ispp-g5.github.io/| | 
| GH backend       |https://github.com/ISPP-G5/NexONG_Backend||
| GH frontend      |https://github.com/ISPP-G5/NexONG_Frontend|              |
| GH documentación |https://github.com/ISPP-G5/NexONG|              |
| Clockify         |[https://app.clockify.me/shared/66085b400f0fa031f07dd478](https://app.clockify.me/shared/660996276cf4e742fab78a5b)|              |
| Video demo       | |La demo está en la última release del repositorio de documentación|
| Plataforma de despliegue       | | Carlos Müller ha sido añadido a través del correo proporcionado en el anterior Sprint |

## 3. PPL
Durante el PPL, no se ha vuelto a desplegar nuestra aplicación. Se redesplegará en el WPL.

## 4. WPL
El único cambio sustancial de este despliegue es la participación de voluntarios en clases y eventos. Este cambio está explicado en su correspondiente sección. Los principales cambios han sido la refinación de nuestros casos de usos y arreglos de bugs. 
### 4.1 Mapeo de los usos core
Estos son nuestros casos de uso core:
- **Panel de administrador**
	- *Administración de voluntarios:* deben hacer operaciones RUD con voluntarios, además pueden aceptar o rechazar solicitudes, y descargar en un ZIP los documentos adjuntados en el proceso de registro por el voluntario.
	- *Administración de educadores:* deben hacer operaciones CRUD con educadores. 
	- *Administración de socios*: deben hacer operaciones RUD con socios y crear asambleas. Además, es posible descargar las donaciones en PDF, CSV o Excel.
	- *Administración de familias:* deben ver a las familias y a sus hijos y aceptar/denegar solicitudes de éstas. 
	- *Administración de clases:* deben hacer operaciones CRUD con clases.
	- *Administración de eventos:* deben poder hacer operaciones CRUD con eventos. La diferencia entre un evento y una actividad es que las actividades están asociadas a una clase.
	
- **Página home:** diferentes ventanas navegables en las que la ONG puede anunciar su labor. 
- **Operaciones no matchmaking:** 
	- *Registro:* en nuestra aplicación te puedes registrar como voluntario, familia o socio.
	- *Pago:* en la página de "Donaciones" cuando no se ha iniciado sesión, existen las **Donaciones puntuales**. Como tarjeta de prueba puede usar 4242 4242 4242 4242 como número de tarjeta, 12/29 como fecha de caducidad y 123 como CVC.
	- *Consumo:* iniciando sesión como cualquier tipo de usuario, se podrá consumir nuestro servicio. En la siguiente sección, se listarán todos los servicios que se pueden consumir y como hacerlo.

### 2.2 Información necesaria para la prueba
#### Pantallas a probar (incluyendo credenciales)
- La URL del **despliegue del frontend** es [esta](https://nexong-wpl-page.oa.r.appspot.com/).
- La URL del **despligue del backend** es [esta](https://nexongapi-wpl.ew.r.appspot.com/api). Además, puede ver su documentación en Swagger [aquí](https://nexongapi-wpl.ew.r.appspot.com/docs).

>[!NOTE]
>Podría ocurrir que al entrar en alguno de los dos despliegues diera un `Server Error`. Esto se daría en caso de que los créditos se hubieran consumido. Estaremos atentos a que esto no pase, pero, si ocurriera, por favor avísennos.

**Página de Inicio**
- Pueden navegar a través de las diferentes pantallas.
- Pueden hacer donaciones puntuales y sugerencias.

**Panel de administrador**
Inicia sesión con las credenciales **info.nexong@gmail.com/m4n0s4bi3rt4sc0nn0rt3**.  
- _Perfil_: puedes ver el perfil de administrador y actualizarlo.  
- _Voluntarios_: puedes verlos, borrarlos y editarlos.
- _Voluntarios > Solicitudes_: puedes ver/aceptar/rechazar y descargar un zip con los documentos de las solicitudes de los voluntarios. 
- _Educadores_: puedes verlos, borrarlos y editarlos. 
- _Educadores > Añadir educador:_ puedes crear un educador.
- _Socios_: puedes verlos, borrarlos y editarlos. También, puedes descargar todos las donaciones en formato pdf, excel o csv y convocar una asamblea. 
- _Familias_: puedes ver las familias y la información de sus hijos  
- _Familias > Solicitudes_: puedes ver/aceptar/rechazar y descargar un documento pdf de las solicitudes de nuevos niños.  
- _Clases_: puedes verlas, editarlas y borrarlas. 
- _Clases > Crear clase_ : puedes crear una clase.
- _Clases > Crear horario_ : puedes crear un horario para la clase.
- _Eventos_: puedes verlos, crearlos, borrarlos y editarlos (si creas un evento haciendo click en el calendario, la fecha de inicio se pone automáticamente).  
- _Sugerencias:_ puedes verlas y borrarlas.  
- _Documentos_: aquí se suben los documento que aparecen en la página "Transparencias" de la página de inicio. Al añadir el documento, este se podrá ver en la tabla de la página mencionada y al hacer click se puede descargar este documento.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de voluntarios**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como voluntario" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**). Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta. Revise el Spam.
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro. 
-  _Formulario_: el usuario, al ser un nuevo voluntario, debe completar el formulario con la información. Los botones de descarga son los documentos que el usuario debe subir rellenados y firmados (excepto el de delitos sexuales que explica como conseguir ese documento). Si el voluntario es menor de edad, tendrá que subir dos documentos más (aparece automáticamente). **SOLO SUBIR ALGÚN ARCHIVO PDF, NO HACE FALTA SUBIR DICHOS DOCUMENTOS FIRMADOS.** La fecha de incorporación no es necesaria. Tras completarlo, una pantalla de espera aparecerá y el voluntario permanecerá ahí hasta que sea aceptado. Si es rechazado, el estado cambiará pero la página seguirá activa.  
- **CIERRE SESIÓN e inicie sesión como administrador con las credenciales anteriores**: En Voluntarios > Solicitudes, acepte la solicitud del voluntario creado. Aquí puedes descargar el zip con los documentos.  
- **CIERRE SESIÓN e inicie sesión con las credenciales del voluntario otra vez**: Ahora el voluntario puede ver su pantalla.

>[!WARNING]
>Respecto a las credenciales que se presentan a partir de aquí; hay que tener en cuenta que estos usuarios se han creado a partir de un `python manage.py loaddata populate.json`. Con lo cual, estos usuarios no contienen archivos reales y toda acción que manipule esos archivos pueden dar problemas. Por ello, recomendamos usar los usuarios recién creados.

**Panel de voluntarios**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **mcast@gmail.com/contraseña**.
- _Agenda_: Puede ver, apuntarse y desapuntarse a eventos, a actividades y a clases.  
- _Perfil_: puede actualizar la información. También, **puede borrar los datos de la página web (derecho al olvido) lo cual necesitamos hacer para continuar testeando, ya que no podrá crear otra cuenta con el mismo correo**.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de familias**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como familiar" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).   
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro.

**Panel de familia**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **annanna@gmail.com/contraseña**.
- *Niños:* Puedes ver a tus hijos. Puedes registrar a hijos, que deberán ser aceptados/rechazados por el administrador, como los voluntarios.
- *Evaluación diaria:* Puedes ver las evaluaciones diarias de cada hijo. 
- *Evaluación anual:* Puedes ver las evaluaciones anuales de cada hijo. 
- *Autorizaciones:* Puedes subir las autorizaciones para eventos de cada hijo. Además de ver autorizaciones anteriores y ver actividades disponibles.
- *Calendario:* Puedes ver las clases, eventos y actividades de los hijos.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de socios**
-  _Registro_: vaya a la página "Registrarse" de la página de inicio. Complete los campos, seleccione "Registrarse como socio" y acepte los términos (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).   
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro.

**Panel de socio**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **esteban@gmail.com/contraseña**.
- *Calendario:* puede ver los eventos y las asambleas.
- Tras probar la funcionalidad completa, _Cierre Sesión_ y avance a la siguiente sección.

**Registro de educadores**
- Inicia sesión con la cuenta de administrador.
-  _Educadores > Añadir educador:_ puedes crear un educador, ya que los educadores no se registran en la página (**UTILICE UN CORREO AL QUE PUEDA ACCEDER**).
- Le llegará un correo de info.nexong@gmail.com con un link para activar la cuenta.   
-  _Iniciar sesión_: con el correo y contraseña introducidos en el registro. 

**Panel de educador**
- Puede entrar con el usuario recién creado o puede entrar con las credenciales **palomino@gmail.com/contraseña**.
- Puedes ver un listado de los niños asociados a clases asociadas con tu usuario de educador.
- Puedes ver los datos de contacto de los niños.
- Puedes poner un comentario en cada evaluación, sin embargo, aún no puedes poner nota.
- Puedes ver la asistencia de los alumnos a futuras actividades.
- Tras probar la funcionalidad completa, _Cierre Sesión_.

#### Otras URL solicitadas

|                  | URL | Observations |
|------------------|-----|-|
| Landing page     |https://ispp-g5.github.io/| | 
| GH backend       |https://github.com/ISPP-G5/NexONG_Backend||
| GH frontend      |https://github.com/ISPP-G5/NexONG_Frontend|              |
| GH documentación |https://github.com/ISPP-G5/NexONG|              |
| Clockify         |[https://app.clockify.me/shared/66085b400f0fa031f07dd478](https://app.clockify.me/shared/660996276cf4e742fab78a5b)|              |
| Video demo       | |La demo está en la última release del repositorio de documentación|
| Plataforma de despliegue       | | Carlos Müller ha sido añadido a través del correo proporcionado en el anterior Sprint |
