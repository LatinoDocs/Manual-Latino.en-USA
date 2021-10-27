.. _novedadesLink:

.. meta::
   :description: Novedades y mejoras en la nueva version de Latino
   :keywords: manual, documentacion, latino, novedades

==========
What's new?
==========

Latino version |LATINO_VERSION|
-----------------------------------
This version was released on October 10th, 2020

Impromevents and releases:
+++++++++++++++++++++

----

Improvements:
~~~~~~~~~

----

General commands:
********************
  * The command **imprimirf()** has been fixed on Windows
  * The command **error()** has been fixed on Windows
  * The commands **imprimirf()** and **cadena.formato()** has been improved
      * It has support for recognizing octal, hexadecimal values, and scientific expressions.
      * Octal, hex, and scientific expression values must be enclosed in quotes (a string).
  * Fixed issue with single quotes in strings

Lib "archivo"
**************
  * The command **archivo.crear()** has been fixed
  * The command **archivo.duplicar()** has been improved
  * The command **archivo.renombrar()** has been fixed

Lib "cadena"
*************
  * The command **cadena.reemplazar()** has been fixed
  * The command **cadena.recortar()** has been fixed on Windows
  * The command **cadena.rellenar_izquierda()** has been fixed on Windows

Lib "lista"
************
  * The command **lista.concatenar()** has been fixed
  * The command **lista.insertar()** has been fixed

Lib "mate"
***********
  * The command **mate.aleatorio()** has been improved

Lib "sis"
**********
  * The command **sis.iraxy()** has been fixed on Windows

----

What's new?:
~~~~~~~~~~~

----

Lib "archivo"
**************
  * The command **archivo.anexar()** has been added
  * An alias for the command **archivo.eliminar()** has been added, and its new alias is **archivo.borrar()**
  * The command **archivo.poner()** has been renamed to **archivo.escribir()**
  * The command **archivo.copiar()** has been renamed to **archivo.duplicar()**

Lib "cadena"
*************
  * The command **cadena.regex()** has been renamed to **cadena.regexl()**
  * The command **cadena.match()** has been renamed to **cadena.regex()**

Lib "dic"
**********
  * The command **dic.eliminar()** has been added
  * The command **dic.contiene()** has been added

Lib "lista"
*************
  * The command **lista.separar()** has been added

Lib "mate"
***********
  * The command **mate.acosh()** has been added
  * The command **mate.asenh()** has been added
  * The command **mate.atanh()** has been added
  * The command **mate.pi()** has been added
  * The command **mate.max()** has been added
  * The command **mate.min()** has been added
  * The command **mate.raizc()** has been added
  * The command **mate.tau()** has been added
  * The command **mate.e()** has been added
  * The command **mate.trunc()** has been added
  * A new alias for the command **mate.aleatorio()** has been added and it's **mate.alt()**
  * The command **mate.redondear()** and its alias **mate.rnd()** have been added
  * The commands **mate.base()**, **mate.parte()** and **mate.porc()** have been added

Lib "sis"
**********
  * The command **sis.usuario()** has been added on Windows