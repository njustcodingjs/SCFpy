SCFpy
====================================================
SCFpy is a simple restricted Hartree-Fock code for small molecules
and small basis sets.
The purpose of this program is for computational chemistry beginner students
to understand the concept of RHF and SCF procedure and how they works in the
code.

You can use SCFpy to calculate small molecule energy:

::

    $SCFpy -c 0 -b sto-3g h2.xyz
    >Total SCF energy = -1.06609574024

Installation
------------
::

    pip install SCFpy

or

::

    git clone https://github.com/pudu1991/SCFpy.git
    python setup.py install

Usage
-----

::

    usage: scfpy [-h] [-c CHARGE] [-b BASIS] [-v] [input]

    SCFpy: simple restricted Hartree-Fock code

    positional arguments:
    input                 xyz file of molecule

    optional arguments:
    -h, --help            show this help message and exit
    -c CHARGE, --charge CHARGE
                        specify total charge of the molecule (default: 0)
    -b BASIS, --basis BASIS
                        specify basis set (default: sto-3g)
    -v, --version         displays the current version of SCFpy

Author
------

-  Pu Du (`@pudu.io <http://pudu.io>`_)

Notes
-----
- You have to have NWChem package installed on your machine.
- SCFpy get the total number of electrons, kinetic, potential, overlap, two electrons
integrals from NWChem output.

Troubleshooting
---------------