.. _alogicoLink:

.. meta::
   :description: Función base alogico() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, alogico

============
alogico( )
============
The **alogico\( \)** function converts the numbers and texts to a logical value (**verdadero** o **falso**).

Any number other than **0**, whether it is a positive, negative, or decimal number, will return **verdadero** .

In the same way any text even if this is a blank space will return **verdadero**.

The **alogico\( \)** function will return **falso** only if the number is **0**, if there is nothing in the quotes, or if we assign a **nulo** value.

**Example**

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir(alogico(1))             //Returns "verdadero"
   escribir(alogico(-1))            //Returns "verdadero"
   escribir(alogico(3.14))          //Returns "verdadero"
   escribir(alogico("Hola"))        //Returns "verdadero"
   escribir(alogico(" "))           //Returns "verdadero" (having a blank space makes it "verdadero")
   escribir(alogico("0"))           //Returns "falso"
   escribir(alogico(nulo))          //Returns "falso"
   escribir(alogico(""))            //Returns "falso"</code></pre>