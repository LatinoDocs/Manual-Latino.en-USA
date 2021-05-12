.. meta::
   :description: Latino documentation, the first functional programing language with Spanish syntax
   :keywords: manual, documentation, latino

.. epigraph::
   
   Have been programing for over four decades. Each programmer needs to be responsible for documenting, testing and debugging what they have created - who else knows it better?

   -- Prem Sobel

----

==================================================
Manual Latino |LATINO_VERSION| (English version)
==================================================
Welcome to the documentation of Latino_, the first functional programing language with Spanish syntax.

:Author:
  `Melvin Guerrero`_

:Translator:
  `Melvin Guerrero`_

:Version:
  `Latino 1.3.0`_

Getting Started
----------------

.. container:: tocdescr
   
   .. container:: descr
      
      :doc:`/About-Latino`
   
   .. container:: descr
      
      :doc:`/Instalar-Latino`
   
   .. container:: descr
      
      :doc:`/Editores-Textos`
   
   .. container:: descr
      
      :doc:`/ejemplos/Mi-Primer-Programa`

Categories
-----------

.. container:: tocdescr
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_novedades.png
         :target: Novedades.html

      :doc:`/Novedades`
         Discover whats new in this version of Latino |LATINO_VERSION|
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_operadores.png
         :target: sintaxis/Operadores.html

      :doc:`/sintaxis/Operadores`
         Arithmetic, assignment, conditional, logical, relational operators, and more.
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_datos.png
         :target: sintaxis/Tipos-de-Datos.html

      :doc:`/sintaxis/Tipos-de-Datos`
         Data types is a classification that defines the value associated with a variable or object.
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_cadena.png
         :target: sintaxis/Cadenas.html

      :doc:`/sintaxis/Cadenas`
         Strings are used to store and manipulate text in Latino.
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_modulo.png
         :target: sintaxis/Modulo.html

      :doc:`/sintaxis/Modulo`
         A module is a file that contains a set of functions that you want to include in your application.
   
   .. container:: descr
      
      .. figure:: /_static/_media/indice/index_regex.png
         :target: sintaxis/RegEx.html

      :doc:`/sintaxis/RegEx`
         A Regular Expression or RegEx is a sequence of characters that form a search pattern.
   
   .. container:: descr
      
      :doc:`/Funciones-Base`
         They are predefined functions that help us perform certain tasks.
      
   .. container:: descr
      
      :doc:`/latGlosario`
         List of libraries, reserved words and definitions in Latino.

----

Other Documentations
----------------------
`Latino API`_ (On development)

----

External links
-----------------
`Youtube channel`_ (Spanish only)

`Latino on-line editor`_

.. attention:: This documentation is subject to modifications and updates because is still in development. Thank you.

==================
Get Involved
==================
This manual is open to anyone who wants to collaborate.

Please, if you which to help see the `collaboration guide`_.


.. Enlaces

.. _Latino: https://lenguajelatino.org
.. _Melvin Guerrero: https://melvinguerrero.blogspot.com
.. _Latino 1.3.0: https://github.com/lenguaje-latino/Latino/releases/tag/v1.3.0
.. _Latino API: https://manuallatinoapi.blogspot.com
.. _collaboration guide: https://github.com/LatinoDocs/Manual-Latino.en-USA/blob/master/.readme/CONTRIBUTING.md
.. _Youtube channel: https://www.youtube.com/channel/UCLVTJpQn-TDbBSwR732kvnQ/featured
.. _Latino on-line editor: https://editorlatino.blogspot.com

.. Tabla de contenido (TOC)

.. toctree::
   :maxdepth: 2
   :hidden:
   
   Introduction
   About-Latino
 
.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Install Latino

   OS/MS-Windows
   OS/Debian-Ubuntu
   OS/Fedora-CentOS
   OS/macOS-X

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Text editors

   editores/Atom
   editores/Notepad++
   editores/Sublime-Text
   editores/TextMate
   editores/Vim
   editores/VS-Code 

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: First steps

   ejemplos/Mi-Primer-Programa

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Syntax

   sintaxis/Comentarios
   sintaxis/Variables
   sintaxis/Operadores
   sintaxis/Aritmetica
   sintaxis/Asignacion
   sintaxis/Relacionales
   sintaxis/Logicos
   sintaxis/Tipos-de-Datos
   sintaxis/Numeros
   sintaxis/Cadenas
   sintaxis/Funciones
   sintaxis/Lista
   sintaxis/Diccionarios
   sintaxis/Condicion-Si
   sintaxis/Condicion-Elegir
   sintaxis/Condicion-Desde
   sintaxis/Condicion-Mientras
   sintaxis/Condicion-Repetir
   sintaxis/Modulo
   sintaxis/RegEx

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Main functions (internal)
   
   funciones/acadena
   funciones/alogico
   funciones/anumero
   funciones/imprimir
   funciones/imprimirf
   funciones/incluir
   funciones/leer
   funciones/limpiar
   funciones/tipo

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Library

   librerias/Archivo
   librerias/Cadena
   librerias/Diccionario
   librerias/Lista
   librerias/Matematica
   librerias/Sistema

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Console

   consola/Comandos-Consola

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: References

   latGlosario
