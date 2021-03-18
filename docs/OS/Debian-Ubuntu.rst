.. _debianLink:

.. meta::
   :description: Steps to follow for installing Latino on Debian and Ubuntu
   :keywords: installation, latino, debian, ubuntu, linux

===============
Debian - Ubuntu
===============
To install Latino on Debian or Ubuntu , first open the console (Terminal) and execute the following commands:

.. code-block:: bash

   sudo apt-get update
   sudo apt-get install git bison flex cmake gcc g++
   sudo apt-get install libcurl4-openssl-dev libhiredis-dev libjansson-dev
   sudo apt-get install redis-server curl libgtk-3-dev
   sudo apt-get install libreadline-dev libpthread-stubs0-dev

.. note:: The code above is **LIBCURL4**, not LIBCUR14

Once this is over, we move on to installing Latino itself in our system

.. code-block:: bash

  cd ~
  sudo git clone --recursive https://github.com/lenguaje-latino/Latino
  cd latino
  sudo git submodule update --init --recursive
  sudo cmake .
  sudo make
  sudo make install

**... and ready!** to run Latino we only need to write in our terminal the **latino** command

.. note:: If in the process of installing **Latino** on **Debian or Ubuntu** causes any problems or conflicts, feel free to look for the solutions `here`_


.. Links

.. _here: https://es.stackoverflow.com/questions/tagged/latino
