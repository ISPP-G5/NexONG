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
1.0.0 | 7/4/2024 | Semana 9 | PEDRO LÓPEZ RUZ Y SAMUEL LUIS RODRÍGUEZ MANESS | MARÍA NÚÑEZ REYES



## Introducción
Este documento recopila los problemas encontrados a lo largo de todo el proceso de desarrollo del proyecto. Por cada problema se especifica el conflicto en sí, cuando se dio, cómo (y cuándo) se resolvió y el impacto que tuvo sobre el proyecto.

Este historial no debe sólo informar sobre el historial del desarrollo de la aplicación, si no también servir como referencia para futuros problemas y poder actuar en concordancia a ellos.

## Registro

### Problemas con los permisos de algunas funcionalidades

Durante la realización de los test varios compañeros se dieron cuenta que faltaban permisos para una serie de funcionalidades como por ejemplo la creación de familias. Tras investigar la causa se comprobó que provenía de una implentación, la cual, trataba de adjuntar los permisos admin de las aplicaciones pero durante el desarrollo de la misma omitió algunos permisos provocando errores. Debido a esto el fronted no puedo trabajar de manera fluida debido que se les impedían realizar varias funciones para probar sus métodos implemetados.
 

## Soluciones
Las soluciones que se pondrán o ya se han puesto en marcha para resolver los problemas anteriores son los siguientes:

- Tras localizar los errores se lanzó una rama hotfix que corregía dichos permisos y se lanzó una pull request para comprobar que verdaderamente se había realizado el cambio.

## Resultados

Los resultados tras la aplicación de las soluciones

- Una vez aceptada la pull request y integrada en la rama develop el frontend pudieron trabajar sin ningun tipo de problema.


