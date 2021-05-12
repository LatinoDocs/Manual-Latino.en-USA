.. _fedoraLink:

.. meta::
   :description: Steps to install Latino on Fedora and CentOS
   :keywords: installation, latino, fedora, centos, linux

================
Fedora - CentOS
================
To install Latino on Fedora or CentOS, first open the console (Terminal) and run the following commands:

.. tabs::
   
   .. tab:: Fedora 26
      
      .. code-block:: bash

         sudo dnf update
         sudo dnf install gcc-c++
         sudo dnf install git bison flex cmake kernel-devel
         sudo dnf install readline-devel

   .. tab:: Fedora 25
      
      .. code-block:: bash
      
         sudo dnf update
         sudo dnf install gcc-c++
         sudo dnf install gtk3-devel
         sudo dnf install git bison flex cmake kernel-devel
         sudo dnf install hiredis-devel
         sudo dnf install readline-devel
      
   .. tab:: Fedora 24
      
      .. code-block:: bash
      
         sudo dnf update
         sudo dnf install bison flex cmake gcc g++ libjansson-dev libcurl4-openssl-dev libhiredis-dev redis-server curl jansson-devel groupinstall "Development Tools" "Development Libraries" groupinstall "RPM Development Tools" redhat-lsb libgtk-3-dev gtk3-devel readline-devel

Once this is over, we move on to installing Latino onto the machine

.. code-block:: bash
   
   cd ~
   sudo git clone --recursive https://github.com/lenguaje-latino/Latino
   cd latino
   sudo git submodule update --init --recursive
   sudo cmake .
   sudo make
   sudo make install

**... and ready!** to run Latino we just write in our terminal the command **latino**

.. note:: If installing **Latino** in **Fedora or CentOS** causes any problems or conflicts, feel free to look for solutions in the forum `here`_


.. Links

.. _here: https://es.stackoverflow.com/questions/tagged/latino