Installation
============

Download the `MassCCS <https://github.com/cepid-cces/massccs>`_ or clone the repository on your computer::

    git clone https://github.com/cepid-cces/massccs.git


Required Software
~~~~~~~~~~~~~~~~~

Pypka depends on the following software:

* C++9.3+
* Boost library 1.60.0+
* CMake 3.13+

On Ubuntu/Debian, you can simply run the following commands to install them with the package manager::

  sudo apt install gcc
  sudo apt-get install -y libboost-filesystem-dev libboost-thread-dev
  sudo apt-get install cmake

Installing
~~~~~~~~~~
.. _label:

This software uses CMake 3.13+ as its build system generator. On your terminal, run the following commands to compile the source code::
    
    cd massccs
    mkdir build # Create build directory    
    cd build    
    cmake .. # Generate Makefiles
    make -j4 # Compile the program

There are optional compilation option that can be used, to see a list of all of them run ``cmake -LH ..``