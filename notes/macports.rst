Arto's Notes re: MacPorts
=========================

http://en.wikipedia.org/wiki/MacPorts

C++11 Development Environment
-----------------------------

::

   $ sudo port install gcc48
   $ sudo port select --set gcc mp-gcc48
   
   $ sudo port install boost +gcc48 -python27

::

   $ sudo port install clang-3.4
   $ sudo port select --set clang mp-clang-3.4
   $ sudo port select --set llvm mp-llvm-3.4
   
   $ sudo port install boost +clang34 -python27

.. note::

   Boost 1.55.0 built with Clang 3.4 presently needs the patch in `#42282`_.

.. _#34288: https://trac.macports.org/ticket/34288
.. _#38374: https://trac.macports.org/ticket/38374
.. _#42282: https://trac.macports.org/ticket/42282