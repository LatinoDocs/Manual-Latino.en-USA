.. _incluirLink:

.. meta::
   :description: Función base incluir() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, incluir

============
incluir( )
============
The **incluir\( \)** function allows you to import **modules** and **libraries** in your project.

When we write the module or library, it must be written in **quotes** and it is not necessary to write its file extension.

**Syntax**

 .. raw:: html
    
    <pre><code class="language-latino line-numbers">incluir("librería")              //It doesn't require a variable
    
    variable = incluir("módulo")     //Require to be assigned to a variable</code></pre>

.. note:: This function can only include files with a **.lat** extension or library files that have been written for Latino and that use its API.

----

Subdirectory
-----------------
With **incluir\( \)**, specifying files in subdirectories varies depending on the operating system.

on MS-Windows, to specify a file in a subdirectory use  **\\**.

On Linux and Mac, to specify a file in a subdirectory use **\/**.

**Example**

To add a file from the following **folder / module** subdirectory, specify it as follows:

.. code-block:: bash
   
   incluir("folder\module")     //MS-Windows
   incluir("folder/module")     //Unix

.. Incluir librerías
.. ------------------
.. Una librería_ es un conjunto de módulos que nos proporciona una serie de funciones/métodos muy concretos que nos ayudan a simplificar tareas complejas y no perjudica la estructura de nuestro código.

.. A diferencia de los módulos en latino, las librerías no requiere ser almacenadas en una variable.

.. ----



.. Enlaces

.. .. _librería: https://es.wikipedia.org/wiki/Biblioteca_(informática)