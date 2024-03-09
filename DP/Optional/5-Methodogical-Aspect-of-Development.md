# &nbsp;&nbsp;&nbsp;&nbsp; Aspecto metodológico del desarrollo - Devising a Project


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
2. Estándares de programación
   1. General
   2. Django
   3. React
3. Estructura del proyecto
4. Política de commits
5. Estrategia de ramas
6. Análisis de código
7. Bibliografía


## Registro de cambios

<table>
  <tr>
   <td><strong>Versión</strong></td>
   <td><strong>Fecha</strong></td>
   <td><strong>Descripción</strong></td>
  </tr>
  <tr>
   <td>1.0.0</td>
   <td>14/2/2024</td>
   <td>Primera versión</td>
  </tr>
  <tr>
   <td>1.1.0</td>
   <td>15/2/2024</td>
   <td>Revisión de apartados</td>
  </tr>
</table>


<br/>

# 

<br/>


# 1. Introducción

Este documento tiene como objetivo establecer pautas claras y consistentes para el desarrollo de software en nuestro equipo, con el fin de garantizar la calidad del código, la eficiencia en el desarrollo y la colaboración efectiva entre todos los miembros del equipo.

A lo largo de este documento, abordaremos varios aspectos clave del desarrollo de software, incluyendo estándares de programación, estructura de proyecto, política de commits y estrategia de ramas. Estas áreas son fundamentales para mantener un código limpio, fácil de mantener y escalable, así como para facilitar un flujo de trabajo colaborativo y organizado dentro del equipo.



# 2. Estándares de programación

## General

- Usa 4 espacios (no tabs) por indentación.
- Se usará únicamente inglés para el código y los comentarios.
- Minimizar comentarios. Siempre intentar explicar el código con el propio código. Por ejemplo, en vez de utilizar una variable ‘i’ y comentar para explicar su función, usar una variable más descriptiva.
- Usa `// FIXME:` para anotar problemas.
- Usa `// TODO:` para anotar soluciones a los problemas.

<img src="images/metodo-desarrollo-general.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />


## Django

- Las líneas de continuación deben alinearse verticalmente con el carácter que se ha utilizado (paréntesis, llaves, corchetes):

<img src="images/metodo-desarrollo-django-1.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- El paréntesis / corchete / llave que cierre una asignación debe estar alineado con el carácter inicial de la primera línea:

<img src="images/metodo-desarrollo-django-2.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Separa funciones de alto nivel y definiciones de clase con dos líneas en blanco. Definiciones de métodos dentro de una clase son separadas por una línea en blanco.
- Usa no más que 1 línea en blanco dentro de funciones para indicar secciones lógicas.
- Las importaciones deben estar en líneas separadas, al comienzo del archivo y ordenadas de la siguiente manera
  1. Importaciones de la librería estándar
  2. Importaciones terceras relacionadas
  3. Importaciones locales de la aplicación / librería
- Siempre usar ruta absoluta para las importaciones
- Evita usar espacios en blanco extraños en las siguientes situaciones:

<img src="images/metodo-desarrollo-django-3.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Siempre rodea estos operadores binarios con un espacio en cada lado: asignación (=), asignación de aumentación (+=, -=, etc.), comparaciones (==, &lt;, >, !=, &lt;>, &lt;=, >=, in, not in, is, is not), “Booleans” (and, or, not).
- Si se utilizan operadores con prioridad diferente, considera agregar espacios alrededor del operador con la menor prioridad. (Usar propio criterio)

<img src="images/metodo-desarrollo-django-4.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Utiliza snake_case para nombrar variables y funciones. Utiliza CamelCase para nombrar clases y métodos. Utiliza minúsculas y guiones bajos para los nombres de archivos y directorios. Las constantes deben estar en mayúsculas.


## React

- No usar [palabras reservadas](http://es5.github.io/#x7.6.1) para nombres de propiedades. Usa sinónimos legibles en lugar de palabras reservadas

<img src="images/metodo-desarrollo-react-1.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Usa comillas simples `''` para las cadenas de texto.
- Usa la notación de punto `.` cuando accedas a las propiedades.

<img src="images/metodo-desarrollo-react-2.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Usa la notación subscript `[]` cuando accedas a las propiedades con una variable.

<img src="images/metodo-desarrollo-react-3.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Siempre usa `var` para declarar variables. No hacerlo resultará en variables globales.

<img src="images/metodo-desarrollo-react-4.png" alt="alt_text" style="width: 50%; display: block; margin: 0 auto;" />

- Usa una declaración `var` por variable.
- Asigna variables al inicio de su ámbito y no en cualquier lado del código. Ejemplo: Si para un bucle necesitas usar una variable nueva, créala justo antes del bucle.
- Usa `===` y `!==` en vez de `==` y `!=` respectivamente.
- Usa camelCase cuando nombres tus objetos, funciones e instancias. Usa PascalCase cuando nombres constructores o clases.
- Si creas funciones de acceso usa `getVal()` y `setVal('hello')` en lugar de `val()` y `val('hello')`.
- Si la propiedad es un booleano, usa `isVal()` o `hasVal()`.



# 3. Estructura del proyecto

    project_name/
    │
    ├── backend/                    # Backend Django
    │   ├── project_name/           # Carpeta del proyecto Django
    │   │   ├── settings.py        	
    │   │   └── urls.py            	
    │   │
    │   ├── core/                   # Aplicación Django principal
    │   │	├── models.py          	
    │   │	├── views.py           	
    │   │	└── urls.py            	
    │   ├── app_name/               # Aplicación Django
    │   │	├── models.py          	
    │   │	├── views.py           	
    │   │	└── urls.py            	
    │   │
    │   └── …
    │	
    └── frontend/                    # Frontend React
    	├── public/               	
    	├── src/                  	
    	│   ├── components/          # Componentes React reutilizables
    	│   ├── pages/               # Componentes de páginas React
    	│   ├── App.js               # Componente principal de la aplicación React
    	│   ├── index.js             # Punto de entrada de la aplicación React
    	│   └── ...               	
    	│
    	└── ...                      # Otros archivos de configuración de React


El proyecto se dividirá en dos repositorios, uno para el backend y otro para el frontend. ‘backend’ contendrá todo el código relacionado con Django y ‘frontend’ tendrá el código de React.

- **project_name/**: Es la carpeta principal del proyecto Django.
  - **core/**: Es la aplicación principal, tendrá todos los modelos y funcionalidades comunes y configuraciones compartidas que son utilizadas por las demás aplicaciones.
  - **app_name/**: Es una aplicación Django. Habrá una por cada funcionalidad principal ofrecida por nuestra plataforma.
- **public/**: Contiene archivos públicos de React, como el index.html.
- **src/**: Contiene el código fuente de la aplicación React.
  - **components/**: Carpeta para componentes React reutilizables.
  - **pages/**: Carpeta para componentes de páginas React.
  - **App.js**: Componente principal de la aplicación React.
  - **index.js**: Punto de entrada de la aplicación React.

Esta es la estructura básica de partida. Las distintas aplicaciones Django se crearán según se implementen en los sprints. En el código fuente de React se agruparán en carpetas según se necesiten distintos servicios, si interactuamos con la API de Django u otras APIs externas; hooks personalizados, para reutilizar lógica; y otros elementos como constantes, estilos, etc.


# 4. Política de commits

### General:

- Cada commit debe representar un cambio atómico y coherente en el código. Esto significa que un commit debe contener cambios relacionados y no varios cambios no relacionados.
- Realiza commits pequeños y frecuentes en lugar de commits grandes y poco frecuentes. Esto facilita la revisión del código y la identificación de problemas.
- Evita realizar commits que dejen el código en un estado no funcional o roto.

### Formato:

- Se deberá separar el título del cuerpo por una línea vacía.
- El título no podrá tener más de 50 caracteres.
- No se pondrá un punto al final del mensaje.
- En el resumen deberá indicar el qué y/o el por qué se ha hecho, no el cómo.
- La primera letra tanto para el título como para el resumen deberá de estar en mayúscula.
- Se escribirán todos los commits en inglés.


# 5. Estrategia de ramas

1. **Rama principal (main/master)**:
    * Esta rama debe contener únicamente código que está listo para ser desplegado en producción.
    * Nunca se debe trabajar directamente en esta rama.
    * Solo se deben fusionar cambios a esta rama desde ramas de develop una vez que haya terminado el sprint.
2. **Rama develop (develop)**:
    * Esta rama es la rama principal sobre la que se desarrollan las nuevas funcionalidades.
    * Nunca se debe trabajar directamente en esta rama.
    * Solo se deben fusionar cambios a esta rama desde ramas de características una vez que hayan sido revisadas y aprobadas.
3. **Ramas de características (feature)**:
    * Cada nueva funcionalidad o tarea debe ser desarrollada en su propia rama de características.
    * Las ramas de características deben ser creadas a partir de la rama develop.
    * Deben tener nombres descriptivos que reflejen la funcionalidad que están implementando (por ejemplo, `feature/nueva-autenticacion`).
    * Después de completar el trabajo en una rama de características, se debe abrir una pull request para su revisión.
4. **Ramas de hotfix (hotfix)**:
    * Para abordar problemas críticos en producción, se pueden crear ramas de hotfix a partir de la rama principal.
    * Estas ramas se utilizan para correcciones rápidas que deben ser implementadas en producción de manera urgente.
    * Después de aplicar el hotfix, se debe fusionar en la rama principal.


# 6. Análisis de código

Para analizar el código del repositorio usaremos las siguientes herramientas:

### Github Actions

GitHub Actions es un servicio de automatización que permite crear flujos de trabajo personalizados para automatizar tareas dentro de repositorios de GitHub.

La combinación de estas herramientas permitirá realizar un análisis exhaustivo del código y automatizar procesos de mejora continua. 

### Codacy

Codacy es una plataforma que utiliza análisis estático de código para identificar problemas de calidad del código, vulnerabilidades de seguridad y patrones de diseño incorrectos. Se usará como GitHub Action dentro del repositorio.


# 7. Bibliografía

[https://recursospython.com/pep8es.pdf](https://recursospython.com/pep8es.pdf)

[https://github.com/paolocarrasco/javascript-style-guide/tree/master/es5](https://github.com/paolocarrasco/javascript-style-guide/tree/master/es5)
