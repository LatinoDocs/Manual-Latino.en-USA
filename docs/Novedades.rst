.. _novedadesLink:

.. meta::
   :description: Novedades y mejoras en la nueva version de Latino
   :keywords: manual, documentacion, latino, novedades

==========
Novedades
==========

Versión de Latino |LATINO_VERSION|
-----------------------------------
Esta versión fue liberada el 10 de Octubre, 2020

Mejoras y novedades:
+++++++++++++++++++++

----

Mejoras:
~~~~~~~~~

----

Comandos generales:
********************
  * Se ha corregido el comando **imprimirf()** en MS-Windows
  * Se ha corregido el comando **error()** en MS-Windows
  * Se ha mejorado los comandos **imprimirf()** y **cadena.formato()**
      * Tiene soporte para reconocer valores octales, hexadecimales y expresiones científicas.
      * Los valores octales, hex y expresiones científicas deben de estar entre comillas (una cadena).
  * Se ha solucionado el problema con las comillas simples en las cadenas

Lib "archivo"
**************
  * Se ha corregido el comando **archivo.crear()**
  * Se ha mejorado el comando **archivo.duplicar()**
  * Se ha corregido el comando **archivo.renombrar()**

Lib "cadena"
*************
  * Se ha corregido el comando **cadena.reemplazar()**
  * Se ha corregido el comando **cadena.recortar()** en MS-Windows
  * Se ha corregido el comando **cadena.rellenar_izquierda()** en MS-Windows

Lib "lista"
************
  * Se ha corregido el comando **lista.concatenar()**
  * Se ha corregido el comando **lista.insertar()**

Lib "mate"
***********
  * Se ha mejorado el comando **mate.aleatorio()**

Lib "sis"
**********
  * Se ha corregido el comando **sis.iraxy()** en MS-Windows

----

Novedades:
~~~~~~~~~~~

----

Lib "archivo"
**************
  * Se ha añadido el comando **archivo.anexar()**
  * Se ha añadido un alias al comando **archivo.eliminar()**, y su nuevo alias es **archivo.borrar()**
  * Se ha renombrado el comando **archivo.poner()** por **archivo.escribir()**
  * Se ha renombrado el comanod **archivo.copiar()** por **archivo.duplicar()**

Lib "cadena"
*************
  * Se ha renombrar el comando **cadena.regex()** por **cadena.regexl()**
  * Se ha renombrar el comando **cadena.match()** por **cadena.regex()**

Lib "dic"
**********
  * Se ha añadido el comando **dic.eliminar()**
  * Se ha añadido el comando **dic.contiene()**

Lib "lista"
*************
  * Se ha añadido el comando **lista.separar()**

Lib "mate"
***********
  * Se ha añadido el comando **mate.acosh()**
  * Se ha añadido el comando **mate.asenh()**
  * Se ha añadido el comando **mate.atanh()**
  * Se ha añadido el comando **mate.pi()**
  * Se ha añadido el comando **mate.max()**
  * Se ha añadido el comando **mate.min()**
  * Se ha añadido el comando **mate.raizc()**
  * Se ha añadido el comando **mate.tau()**
  * Se ha añadido el comando **mate.e()**
  * Se ha añadido el comando **mate.trunc()**
  * Se ha añadido un nuevo alias en el comando **mate.aleatorio()** el cual es **mate.alt()**
  * Se ha añadido el comando **mate.redondear()** y su alias **mate.rnd()**
  * Se ha añadido los comandos **mate.base()**, **mate.parte()** y **mate.porc()**

Lib "sis"
**********
  * Se ha añadido el comando **sis.usuario()** en MS-Windows