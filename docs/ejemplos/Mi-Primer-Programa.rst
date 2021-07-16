.. meta::
   :description: Ejemplos básicos de la sintaxis de Latino
   :keywords: manual, documentacion, latino, ejemplo

===================
My First Program
===================

This section of the manual is focused on giving the user a brief sample of some basic functions and operations that can be done in Latino.

To start with each of the examples, you will have to open the terminal of your OS and have Latino to run.

.. note:: To run Latino in the terminal, just type **Latino** and press the Enter key.

.. container:: note

  |  If you write Latino code in a text editor, save the document with the **.lat** extension.
  |  ~Example: **archivo.lat**

.. tabs::
   
   .. tab:: Hello World!
      
      **Hello World** in Latino

      In this example we are going to make a small program. When executed, it will show a message saying  **"Hello World, Latino!"**
      
      To show a message on the screen, use the following command and press Enter

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Hello World, Latino!")</code></pre>

      The result will be:

      .. code-block:: bash
         
         Hello World, Latino!
      
      .. image:: ../_static/_media/ejemplos/miPrimerPrograma/holaMundo.gif
      

   .. tab:: Print a number
      
      **Print a number** (entered by the user)

      In this example, we'll show you, how you can type and store values ​​to a variable and later show it on the screen.

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a number:")
         num=leer()    //here you create a variable and assign it to the function leer()
         escribir("The number entered is: "..num)</code></pre>
      
      .. note:: If you are writing the code directly in the terminal, you can write everything on one line, like this:

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a number:") num=leer() escribir("The number entered is: "..num)</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         Enter a number:
         24
         The number entered is: 24
      
      .. image:: ../_static/_media/ejemplos/miPrimerPrograma/imprimirNumero.gif


   .. tab:: Odd or Even
      
      **Odd or Even in Latino**

      In this example, you are going to create a program that helps us identify when a number (entered by the user) is even or odd.

      **Example 1:**

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a number:")
         num=leer()
         si (num % 2 == 0)     //True if the number is perfectly divisible by 2
           escribir("The number "..num.." is even")
         sino
           escribir("The number "..num.." is odd")
         fin</code></pre>
      
      .. note:: If you are writing the code directly in the terminal, you can write everything on one line, like this:

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a number:") num=leer() si(num%2==0) escribir("The number "..num.." is even") sino escribir("The number "..num.." is odd") fin</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         Enter a number:
         8
         The number 8 is even

      **Example 2:**

      This is another way to create the same program but with a fewer lines of code:

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a number:")
         num=leer()
         escribir("The number "..num..(num%2==0)?" is even":" is odd")</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         Enter a number:
         -7
         The number  -7 is odd

      .. image:: ../_static/_media/ejemplos/miPrimerPrograma/numeroParImpar.gif

   .. tab:: Intercambiar números
      
      **Exchange two numbers between variable in Latino**

     In this example we will make a program that exchanges the values ​​of two variables with each other.
	 
      **Example 1:**

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">firstNum = 2
         secNum = 5
         firstNum, secNum = secNum, firstNum  //Here, the values are exchanged
         escribir("FirstNum:"..firstNum.." | SecondNum:"..secNum)</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         FirstNum:5 | SecondNum: 2
      
      **Example 2:**

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter the first number:")
         firstNum=leer()
         escribir("Enter the second number:")
         secNum=leer()
         tempVar=firstNum    //The value of the first variable is assigned to a temporary variable
         firstNum=secNum     //The value of the second variable is assigned to the first variable
         secNum=tempVar    //The value of the temporary variable is assigned to the second variable
         escribir("After exchanging, the first variable is: "..firstNum)
         escribir("and the second variable is:"..secNum)</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         Enter the first number:
         1
         Enter the second number:
         2
         After exchanging, the first variable is: 2
         and the second variable is: 1
      
      **Example 3:**

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter the first number")
         firstNum=leer()
         escribir("Enter the second number")
         secNum=leer()
         //Exchanging process
         firstNum=firstNum-secNum
         secNum=firstNum+secNum
         firstNum=secNum-firstNum
         escribir("After exchanging, the first variable is "..firstNum)
         escribir("and the second variable is"..secNum)</code></pre>

      The result will be:

      .. code-block:: bash
         
         Enter the first number
         10.25
         Enter the second number
         -12.5
         After exchanging, the first variable is -12.5
         and the second variable is 10.25
      
      .. image:: ../_static/_media/ejemplos/miPrimerPrograma/intercambiarNumeros.gif

   .. tab:: Vowel or consonant
      
      **Identificar si el caracter es vocal o no en Latino**
      
      In this example, you are going to create a program that is capable of knowing if the value you enter is a vowel or a consonant.

      .. raw:: html
         
         <pre><code class="language-latino line-numbers">escribir("Enter a letter")
         alphabet=leer()
         vowels=["a","A","e","E","i","I","o","O","u","U"]    //Vowels declaration

         response = alphabet..", is not a vowel"

         desde (i=0; i < lista.longitud(vowels); i++)
            si (alphabet==vowels[i])
               response = alphabet..", is a vowel"
            fin
         fin

         escribir (response)</code></pre>
      
      The result will be:

      .. code-block:: bash
         
         Enter a letter
         a
         a, es un vocal
      
      .. image:: ../_static/_media/ejemplos/miPrimerPrograma/caracterVocaloNo.gif