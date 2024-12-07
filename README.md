<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

# Mecatronica-Proyecto
<!-- [![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

 -->


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo_con_fondo.png" alt="Logo" width="650" height="200">
  </a>

  <h3 align="center">Proyecto-Zeus.</h3>

  <p align="center">
    <br />
    <a href="https://github.com/RoboTech-URJC/Mano-Zeus.git"><strong>Original Robotech Repo »</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues/new?labels=bug&template=bug-report---.md">Personal Blog</a>
  </p>
</div>


## Sesiones 3-4-5 | Diseño 2D.

En estas sesiones nos centramos en el diseño 2D. He aplicado los conocimientos en clase para diseñar un pequeño logo que decore el proyecto.
Requisitos:
* Inkscape.
* Creatividad.

<div align="center">
  <a>
    <img src="images/logo_con_fondo.png" alt="Logo" width="650" height="200">
  </a>

</div>

A continuacion os dejo un pequeño video de como Marvin ha hecho este pequeño logo sobre el proyecto: 

https://github.com/user-attachments/assets/d4b07c5d-308e-4ce0-a138-df33238a739b

Empleando Inkspace he desarrollado un dibujo de la estructura que debe de tener la mano robótica que vamos a recrear. Es un diseño simple a modo de entendimiento de las diferentes partes que la componen. 

Este es el diseño que hemos obtenido:

<div align="center">
  <a>
    <img src="images/Mano.svg" alt="Mano_svg" width="650" height="400">
  </a>

</div>

<p align="right">(<a href="#readme-top">inicio</a>)</p>

En materia del diseño vectorial, también es posible compatibilizarlo con otras técnicas, y para aplicarlo también al proyecto desde otra perspectiva, se me ha ocurrido investigar conversores de gráficos. Existen numerosos convertidores online gratuitos y algunos otros de pago que mejoran los resultados, y esto facilita que ciertas imágenes o diseños puedan ser vectorizados con herramientas también distintas a Inkscape y que no están pensadas en un principio para el diseño vectorial.

Aplicando estas herramientas a nuestro proyecto, Moisés ha diseñado un dibujo simple de algunos componentes de la mano, que también puede servir de apoyo a diagramas explicativos o información que se quiera enseñar y explicar del proyecto:

<p align="center">
  <img src="images/composicion_dedo.png" alt="Alt Imagen 1" width="49%">
  <img src="images/composicion_dedo_vect_color.svg" alt="Alt Imagen 2" width="49%">
</p>

De las dos imágenes superiores, la izquierda pertenece a un formato en .png, siendo el fichero de dibujo original. Por otra parte la imagen derecha es el resultado de pasar la anterior por un conversor a svg (formato vectorial). El utlizado en este caso ha sido:
- https://png2svg.com/es/

Dejo a continuación un vídeo del proceso de diseño original de la imagen superior, en un programa de diseño no vectorial:

![Time-lapse](./videos/video_diseño_dedo.gif)


## Sesiones 6-7-8-9 | Diseño 3D.

En cuanto al diseño en 3D que hemos implementado en FreeCad ha sido una estructura simple del ejemplo de dibujo en 2D de Inkspace, obteniendo una estructuracompuesta por rectangulos similar a una mano, pero bastante simplificada. Mostrando en ella todos las piezas en las que tenemos pensado estructurarla.

La estructura se encuentra en el siguiente link: [Mano.FCStd](https://github.com/mpancracio2020/Mecatronica-Proyecto/tree/main/images/Mano.FCStd)

En cuanto al resto de diseño 3D hemos utilizado Ultimaker Cura para diseñar las piezas basandonos en el proyecto original del cual hemos sacado la idea. Hemos modificado los archivos (.lts) de los componentes aportando diferentes valores para obtener la mejor impresión de las piezas en nuestras impresoras 3D.

---

# **Diseño Electrónico de la Mano de Zeus**
## 1. Componentes:
Para crear y diseñar el circuito electronico primero debemos elegir que componentes son necesarios y los más óptimos para el correcto funcionamiento de la mano.

- **Arduino UNO / MEGA:** primero hemos elegido como cerebro de nuestro robot un arduino UNO ya que es suficiente para poder comandar el resto de componentes. Si se llega a aumentar el numero de componentes como el añadir otro brazo, usaremos un arduino Mega para poder tener mas pines a los que conectar todos los componentes.
<br>
<image src="https://github.com/vbarcena2020/My_personal_page/blob/master/assets/images/arduinos.jpg?raw=true"></image> 
<br>
- **Servos:** en concreto el modelo tower pro mg996r, un servo de 360 grados el cual nos permite una rotación completa y necesaria para mover los dedos y muñeca los ángulos necesarios. En concreto usaremos 6 servos por cada mano.
<br>
<image src="https://github.com/vbarcena2020/My_personal_page/blob/master/assets/images/servo.jpg?raw=true"></image> 
<br>
- **Protoboard:** Usaremos una protoboard para tener mejor conectados y controlados todos los componentes.
- **Cables Macho-Macho:** para conectar los componentes entre sí.

## 2. Circuito (Fritzing):
Para poder visualizar de una manera mas simple y rapida sin tener que conectar de forma presencial todo el circuito hemos usado la aplicación Fritzing para poder diseñar el circuito. Esta nos permite añadir los componentes necesarios y los modelos específicos que utilizaremos.

El circuito diseñado es el siguiente:
<br>
<image src="https://github.com/vbarcena2020/My_personal_page/blob/master/assets/images/fritzing_design.png?raw=true"></image> 
<br>

---

# Montaje de la Mano de Zeus

## 1. Componentes:

Teniendo el diseño 3d de las piezas, ajustamos adecuadamente los tamaños y utilizamos una impresora 3d para imprimir cada una. En total para la mano derecha desarrollada fueron utilizadas las siguientes partes:
- **Dedo meñique:** conformado por 6 piezas, ensambladas posteriormente entre sí. Adaptado del modelo original: [auriculaire-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=Auriculaire3.stl)
- **Dedo anular:** conformado por 6 piezas, ensambladas posteriormente entre sí. Adaptado del modelo original: [ring-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=ringfinger3.stl)
- **Dedo corazón:** conformado por 6 piezas, ensambladas posteriormente entre sí. Adaptado del modelo original: [majeure-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=Majeure3.stl)
- **Dedo índice:** conformado por 6 piezas, ensambladas posteriormente entre sí. Adaptado del modelo original: [index-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=Index3.stl)
- **Dedo pulgar:** conformado por 6 piezas, ensambladas posteriormente entre sí. Adaptado del modelo original: [thumb-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=thumb5.stl)

<p align="center">
  <img src="images/componentes_dedo.png" alt="componentes_dedo" width="70%">
</p>

- **Espaciador:** soporte estructural para ensamblar los dedos meñique y anular con la muñeca corta. Adaptado del modelo original: [bolt-entretoise](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=Bolt_entretoise7.stl)
- **Muñeca larga:** pieza única, ensamblada para conformar el mecanismo del movimiento transferido de muñeca a los dedos, junto con la Muñeca corta. Adaptado del modelo original: [wrist-large](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=WristlargeV4.stl)
- **Muñeca corta:** dos piezas, ensambladas al dedo anular y meñique, uniéndolos a la Muñeca larga para conformar el movimiento transferido por la muñeca a los dedos mencionados. Adaptado del modelo original: [wrist-small](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=WristsmallV4.stl)

<p align="center">
  <img src="images/wrist_assembly.png" alt="visualización_virtual" width="60%">
</p>

- **CableHolderWristV5:** elemento de apoyo para facilitar la incorporación del cableado que conecta con muñeca y mano. Adaptado del modelo original: [cable-holder](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Rotation-Wrist&parts=CableHolderWristV5.stl)
- **RotaWrist 3V3:** pieza única relacionada con el módulo de la muñeca. Adaptado del modelo original: [rotawrist3v3](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Rotation-Wrist&parts=RotaWrist3V3.stl)
- **RotaWrist 2V3:** primera de las piezas que conforman la cobertura posterior del módulo de la muñeca. Adaptado del modelo original: [rotawrist2v3](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Rotation-Wrist&parts=RotaWrist2V3.stl)
- **RotaWrist 1V4:** segunda de las piezas que conforman la cobertura posterior del módulo de la muñeca. Adaptado del modelo original: [rotawrist1v4](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Rotation-Wrist&parts=RotaWrist1V4.stl)
- **WristgearsV5:** engranajes necesarios para la rotación del módulo de la muñeca. Adaptado del modelo original: [wrist-gears](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Rotation-Wrist&parts=WristGearsV5.stl)
- **RobocableBackV3:** pieza de apoyo para la integración del cableado, junto con rob-cable-front. Adaptado del modelo original: [rob-cable-back](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=RobCableBackV3.stl)
- **RobocableFrontV3v:** segunda pieza de apoyo para la integración del cableado con la rotación de muñeca. Adaptado del modelo original: [rob-cable-front](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=RobCableFrontV3.stl)
- **RoboRingV3:** anillos ensamblados a los servomotores, necesarios para implementar el movimiento de los dedos. Adaptado del modelo original: [rob-ring](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=RobRingV3.stl&doing_wp_cron=1732996341.5229659080505371093750)
- **RobServoBedV6:** pieza única empleada para situar correctamente la posición interna de los servomotores. Adaptado del modelo original: [servo-bed](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=RobServoBedV6.stl)
- **TensionerRightV1:** pieza de apoyo al ensamblaje de los componentes internos. Adaptado del modelo original: [tensioner-right](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=TensionerRightV1.stl)
- **Servo-pulley:** poleas circulares, transforman el movimiento de los servomotores. Adaptado del modelo original: [servo-pulley](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Forearm-and-Servo-Bed&parts=servo-pulleyX5.stl)

<p align="center">
  <img src="images/foto_dorso_mano.jpeg" alt="visualización_virtual" width="45%">
  <img src="images/foto_palma_mano.jpeg" alt="visualización_virtual" width="45%">
</p>

- **Cubierta superior (tumbada):** similar a las piezas que cubren los dedos, siendo esta una cobertura para la parte superior de la mano. Adaptado del modelo original: [top-surface](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=topsurfaceUP6.stl&doing_wp_cron=1732995560.7582659721374511718750)
- **Cubrededos:** conformado por 5 piezas, ensambladas sobre los dedos. Adaptado del modelo original: [cover-finger](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=coverfinger1.stl)
- **Soporte Arduino:** pieza única para contener la placa Arduino controladora. Adaptado del modelo original: [arduino-support](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=ardiuinosupport.stl)
- **Robcap3V2:** uno de los componentes que conforman el antebrazo, siendo la cubierta superior del mismo. Adaptado del modelo original: [robcap3v2](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=robcap3V2.stl)
- **Robcap2V4:** primera cubierta anterior del antebrazo. Adaptado del modelo original: [robcap2v4](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=robpart2V4.stl)
- **Robcap3V4:** segunda cubiera anterior del antebrazo. Adaptado del modelo original: [robcap3v4](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=robpart3V4.stl)
- **Robcap4V4:** primera cubierata posterior del antebrazo. Adaptado del modelo original: [robcap4v4](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=robpart4V4.stl)
- **Robcap5V4:** segunda cubierta posterior del antebrazo. Adaptado del modelo original: [robcap5v4](https://inmoov.fr/inmoov-stl-3d/?bodyparts=Right-Hand&parts=robpart5V4.stl)

<p align="center">
  <img src="images/foto_brazo_completo.jpeg" alt="visualización_virtual" width="65%">
</p>

# **Diseño esquemático por componentes**

Para simplificar el montaje, y describir de manera más sencilla la forma en que se realizó, queda a continuación un diagrama dibujado y comentado, con sus elementos explicados en detalle más adelante en este mismo documento:

<div style="display: flex; align-items: left;">

<div style="flex: 1;">
<img src="images/diagrama_elementos_mano.jpg" alt="diagrama" width="80%">
</div>

<div style="flex: 1;">
<table>
  <tr>
    <th>F1 - F6</th>
    <td>Falanges de la superior a inferior, de todo dedo salvo el pulgar</th>
  </tr>
  <tr>
    <th>T1 - T6</td>
    <td>Falanges de la superior a inferior, del dedo pulgar</td>
  </tr>
  <tr>
    <th>PA</td>
    <td>Pieza intermedia entre la parte central de la mano y el dedo anular. Esta pieza rota en torno a un tornillo que la encaja</td>
  </tr>
  <tr>
    <th>PB</td>
    <td>Pieza intermedia entre la parte central de la mano y el dedo meñique. Esta pieza rota en torno a un tornillo que la encaja</td>
  </tr>
  <tr>
    <th>PC</td>
    <td>Pieza central de la mano sobre la cual se ensamblan los dedos pulgar, índice y corazón, y las piezas intermedias PA y PB</td>
  </tr>
  <tr>
    <th>MR</td>
    <td>Parte rotativa de la muñeca, apoyada sobre la muñeca fija, y ofreciendo movimiento en torno al servomotor interno a la misma</td>
  </tr>
  <tr>
    <th>MF</td>
    <td>Muñeca fija, conjunto de piezas y cobertura que sirven de apoyo a la muñeca rotativa para ejercer su giro</td>
  </tr>
  <tr>
    <th>SVM</td>
    <td>Servomotor de la muñeca. Situado interno a la muñeca fija, y anclado a la rotativa</td>
  </tr>
  <tr>
    <th>AS</td>
    <td>Antebrazo superior. Conjunto de piezas encarcasadas más cortas que el antebrazo posterior, uniendo la muñeca con el mismo</td>
  </tr>
  <tr>
    <th>SLC & SRC</td>
    <td>Esquinas superior izquierda (SLC) y superior derecha (SRC) de la carcasa interna del antebrazo posterior o largo. Deben ir alineadas con ILC e IRC respectivamente</td>
  </tr>
  <tr>
    <th>ILC & IRC</td>
    <td>Esquinas superior izquierda (ILC) y superior derecha (IRC) de la carcasa externa del antebrazo largo. La carcasa de la que forman parte se alinea con la previamente mencionada y la recubre, dando forma al antebrazo</td>
  </tr>
  <tr>
    <th>PC1</td>
    <td>Conjunto de piezas centrales al antebrazo largo, ensambladas sobre la carcasa interna para servir de guía para los cables o fibras que mueven los dedos</td>
  </tr>
  <tr>
    <th>SV1 - SV6</td>
    <td>Servomotores numerados del 1 al 6, Componen el sistema de movimiento de los dedos de la mano, uniéndose a ellos por medio de unas cuerdas (C alpha) ancladas a los servos gracias a unas guías circulares</td>
  </tr>
  <tr>
    <th>SVN</td>
    <td>Abreviatura utilizada para referirse a "cualquier servomotor del antebrazo", pudiendo ser desde SV1 hasta SV6 pero no SVM</td>
  </tr>
  <tr>
    <th>C alpha</td>
    <td>Abreviatura utilizada para referirse a "cualquier cuerda ó fibra encargada de guiar el movimiento de los dedos desde su unión a un servomotor SVN" </td>
  </tr>
</table>
</div>

</div>

Aunque en el diagrama aparecen indicados también una serie de elementos que forman parte del dibujo, y la guía puede ser de ayuda para entender las abreviaturas, hay algunas cosas más que hay que tener en cuenta relativas al montaje: 
- Cada dedo está dividido en el mismo número de falanges, y cada falange cuenta con uniones tanto fijas como rotativas, indicadas estas últimas con un icono explicativo en la imagen superior.
- Las falanges de los dedos, tanto pulgar como índice, corazón, anular y meñique, cuentan con guías para los cables en las uniones articuladas, y con aberturas en aquellas uniones fijas, para que sea posible la unión entre la parte final de cada dedo y el servomotor que lo controlará.
- Además de los tornillos de ensamblaje que se han dibujado arriba, el montaje requirió de la utilización de otros tornillos metálicos no indicados previamente, así como algunos elementos adicionales para la correcta sujeción de algunas piezas.
- La parte interior del antebrazo largo, así como el antebrazo superior en detalle, que se indican previamente y se encuentran explicados, cuentan con otros elementos internos en su estructura, no mencionados por no ser de especial relevancia para la comprensión del funcionamiento del sistema mecánico que conforma la Mano de Zeus

### Esquematización

Queda a continuación un breve time lapse de la **parte final** del diseño del esquema superior:

![time-lapse](./videos/video_diseño_esquema.gif)