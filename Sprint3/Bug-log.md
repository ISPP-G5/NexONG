# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Documento de bugs encontrados - Sprint 3
# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NexOng - Grupo 5



## Índice

1. Introducción
2. Tabla de resultados
3. Conclusión

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
   <td>21/04/2024</td>
   <td>Primera versión</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>MARTA INÉS</td>
  </tr>
</table>



<br/>

# 

<br/>



#  1. Introducción 

Este documento indica los bugs que hemos encontrado al hacer los tests en la aplicación, principalmente recogerá una tabla con los bugs encontrados y la solución que hemos podido obtener gracias a estos.



# 2. Tabla de resultados 

En este apartado vamos a indicar la tabla con los bugs obtenidos al hacer los tests y como gracias a esto hemos podido solventar los diferentes bugs de la aplicación.

<table>
  <tr>
   <td><strong>Bug</strong>
   </td>
   <td><strong>Fecha</strong>
   </td>
   <td><strong>Problema</strong>
   </td>
   <td><strong>Solución</strong>
   </td>
  </tr>
  <tr>
   <td>No se podía crear un partner o un voluntario</td>
   <td>03/04/2024</td>
   <td>El problema es que en los permisos del endpoint, no existían permisos para poder hacer post, por lo tanto no podíamos crearlos</td>
   <td>Se ha puesto permisos de post, además de los demás permisos, para solucionar el problema</td>
  </tr>
</table>

Aquí que que tipo de pruebas hemos hecho

<table>
  <tr>
   <td><strong>Tipo</strong>
   </td>
   <td><strong>Numero de tests</strong>
   </td>
  </tr>
  <tr>
   <td>Unitarios</td>
   <td>93</td>
  </tr>
   <tr>
   <td>Integración</td>
   <td>22</td>
  </tr>
   <tr>
   <td>Carga</td>
   <td>3</td>
  </tr>
</table>



# 3. Conclusión. 

El buen uso de tests, nos pueden indicar diferentes sitios donde encontrar fallos o bugs en la aplicación y solucionarlos, siempre es aconsejable poder hacer varios tests para probar que todo funciona correctamente. Esto debe ser algo básico y correr los test cada vez que hayan cambios en la aplicación para asegurarse que añadiendo cosas nuevas no obstruyes la funcionalidad de ninguna de las cosas necesarias en la aplicación.
