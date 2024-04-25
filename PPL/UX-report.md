# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Análisis de Costes - PPL
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

1. Costes del periodo de desarrollo
   1. Coste salarial del equipo (desarrollo)
   2. Coste derivados del desarrollo
   3. Coste de licencias
   4. Coste de material de trabajo
   5. Costes de marketing durante el periodo de desarrollo
   6. Reservas de contingencia
   7. Desglose total de los costes de desarrollo
2. Costes del periodo de producción
   1. Coste salarial del equipo (producción)
   2. Costes derivados de producción
   3. Costes de licencias en producción
   4. Coste de marketing en producción
   5. Amortización en producción
   6. Desglose total de los costes de producción
3. TCO
4. ROI

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
   <td>1/2/2024</td>
   <td>Completado la primera versión del análisis del coste preliminar del proyecto.</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>CLAUDIA GILABERT PRIETO</td>
  </tr>
  <tr>
   <td>1.0.1</td>
   <td>02/02/24</td>
   <td>Añadido desglose por semana a los costes derivados del desarrollo, nuevas licencias y presupuesto de contingencia.</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>MANUEL ORTIZ BLANCO</td>
  </tr>
  <tr>
   <td>1.0.2</td>
   <td>04/02/24</td>
   <td>Se han desglosado los costes en función de las distintas fases del desarrollo del proyecto. Se ha calculado la amortización de los equipos informáticos. Se ha realizado el análisis de los TCO.</td>
   <td>MANUEL ORTIZ BLANCO</td>
   <td>PEDRO LOPEZ RUZ</td>
  </tr>
  <tr>
   <td>1.0.3</td>
   <td>13/02/24</td>
   <td>Añadidos costes de márketing.</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>MARTA INÉS GONZÁLEZ DIÁNEZ</td>
  </tr>
  <tr>
   <td>1.0.4</td>
   <td>14/02/24</td>
   <td>Añadida más información al documento y el ROI</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>MARTA INÉS GONZÁLEZ DIÁNEZ</td>
  </tr>
  <tr>
   <td>1.0.5</td>
   <td>1/04/24</td>
   <td>Añadida más información respecto al TCO</td>
   <td>FÉLIX ÁNGEL GUDIEL GÜEMES</td>
   <td>MARTA INÉS GONZÁLEZ DIÁNEZ</td>
  </tr>
  <tr>
   <td>1.0.6</td>
   <td>1/04/24</td>
   <td>Añadida más información respecto a la variación del TCO</td>
   <td>FÉLIX ÁNGEL GUDIEL GÜEMES, MIGUEL ANGEL ROMALDE DORADO</td>
   <td>FRANCISCO JAVIER CALDERÓN RODRÍGUEZ</td>
  </tr>
  <tr>
   <td>1.0.7</td>
   <td>24/04/24</td>
   <td>Añadida más información respecto a la variación del TCO</td>
   <td>MIGUEL ANGEL ROMALDE DORADO</td>
   <td>FÉLIX ÁNGEL GUDIEL GÜEMES, FRANCISCO JAVIER CALDERÓN RODRÍGUEZ</td>
  </tr>
</table>

<br/>

#

<br/>

# 1. Introducción

UX (User Experience) hace referencia a la experiencia e impresión que recibe un cliente cuando interactúa con un producto o servicio. En nuestro caso, esta experiencia se centra en la actitud y comportamiento de los futuros clientes de la página web que hemos desarrollado. La UX depende de la aplicación a evaluar y los clientes promedios que recibirá, por lo que no existe un conjunto de pasos a seguir para asegurar que un sistema proporciona una experiencia excelente. Sin embargo, sí que existen un conjunto de métricas que se pueden usar para evaluar la calidad de nuestra aplicación. Antes de aplicarlas, se debe confirmar que son pertinentes para nuestro proyecto y que nos proporcionan información de interés. En este documento se busca investigar sobre estas métricas para comprobar si hemos desarrollado un sistema eficiente y que causa experiencia positiva en sus usuarios.
# 2. Metricas

# 2.1 Retroalimentación de usuarios piloto

La primera y más importante de las métricas a evaluar es la propia opinión de los usuarios. Debemos anteponer el punto de vista de los futuros clientes a cualquier otro tipo de examen de calidad, ya que son nuestro principal indicador de satisfacción. Nuestros usuarios piloto no nos han indicado descontento con la experiencia promedia dentro de la aplicación, por lo que podríamos suponer que nuestra UX es excelente. Sin embargo, esto no es completamente cierto, ya que todos los usuarios piloto han leído una guía sobre la aplicación antes de evaluar el sistema. Si una aplicación tiene una UX sobresaliente, el cliente no necesitaría leer una guía antes de usar nuestra página web, por lo que debemos investigar otras métricas para comprobar la eficacia de nuestro diseño.

Aun así, recibir feedback positivo de nuestros usuarios piloto respecto al diseño es un indicador positivo. Como no disponemos de usuarios de prueba que no conozcan ya la aplicación, investigaremos más métricas para confirmar que, realmente, nuestro diseño es correcto.

# 2.2 Arquitectura de la información (IA)

Esta métrica se refiere a la disposición de la información. La estructura de la información que se muestra en pantalla debería tener forma clara, equilibrada, funcional y escalable. Para poder evaluar esta métrica, nos fijaremos en los desplegables de la página principal y en la barra lateral en los perfiles de usuario. La iconografía en ellas es mínima, por lo que podemos afirmar que la información que se ofrece es clara. Ambas siguen una estructura predeterminada y cautelosamente creada para toda la aplicación, asegurando que está equilibrada y escalable. Además, hemos evitado florituras y cada elemento de estos menús está etiquetado con la sección a la que corresponde, confirmando su funcionalidad.

Podemos entonces afiramr que se ha tenido en cuenta los parámetros descriptores de la Arquitectura de la Información, un indicador de que el diseño de la aplicación es adecuado y correcto.
# 2.3 Prototipos aprobados

Antes de comenzar el desarrollo del proyecto se elaboraron prototipos para todas las pantallas que la aplicación debía contener. Estos prototipos fueron creados por una sección del equipo que conocía de cerca las funcionalidades a implementar y fue revisado por otra parte del equipo, las desconcocía (en su mayoría). Siguiendo este proceso, los revisores emularon a los futuros clientes, ya que no tenían conocimiento previo del sistema. Tras la revisión, el producto final de esta tarea fue un conjunto de prototipos que no sólo cumplían con los requisitos, si no que eran comprensibles para los individuos sin información de la aplicación.

Contando además con el apoyo de los profesores, confirmamos que los prototipos en los que se basa la aplicación final son tanto funcionales como relevantes a la hora de generar una buena UX.
# 2.4 Competencia

Tenemos un diseño similar a blackboard, pero mejor

# 2.5 Mocks centrados en eficacia

Los mocks se hicieron con el cliente promedio en mente

# 2.6 Sencillez del sistema

Se ha antepuesto la funcionalidad a las florituras y los detalles. Para nuestro cliente promedio es bueno

# 3 Conclusión

A partir de los resultados de estas métricas confirmamos que nuestro proyecto cumple con los estándares necesarios para afirmar que posee una UX excelente. Esto implica que nuestros clientes tendrán una experiencia agradable con nuestra aplicación, asegurando claridad, funcionalidad y sencillez. Esto, a su vez, causará que el cliente promedio esté más dispuesto a usar nuestro sistema y que nos ayude a destacar entre el resto de la competencia. Aunque la UX pueda mejorar una vez que se obtenga la retroalimentación del público real del sistema, las métricas que hemos usado nos dan un cierto grado de seguridad en que la experiencia promedia será positiva. 
