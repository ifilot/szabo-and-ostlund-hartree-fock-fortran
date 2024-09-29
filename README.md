# Szabo and Ostlund Hartree-Fock example program

[![build-status](https://github.com/ifilot/szabo-and-ostlund-hartree-fock-fortran/actions/workflows/build.yml/badge.svg)](https://github.com/ifilot/szabo-and-ostlund-hartree-fock-fortran/actions/workflows/build.yml)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

The file [src/hf.f](src/hf.f) contains the source code for a basic Hartree-Fock
(HF) calculation (using the STO-3G basis set) with only s-orbitals, specifically
for the HeH⁺ molecule. 

The source code is obtained from Appendix B of the book "[Modern Quantum
Chemistry](https://store.doverpublications.com/products/9780486691862)", by
Attila Szabo and Neil S. Ostlund. Although the program is written in the older
Fortran 77 language, it can be successfully using the
[gfortran](https://gcc.gnu.org/wiki/GFortran) compiler. A few warnings are being
thrown which can be ignored by the user.

## Compilation instructions

Make sure you have the right dependencies installed

```bash
sudo apt install -y build-essential gfortran
```

After cloning the repository, run

```bash
cd src
make
```

## Running the program

Just type `./hf` to run the program. The output of the program can be found
in [output.txt](output.txt).

## License

With exception of the file [src/hf.f](src/hf.f), all source code provided in
this repository is provided under a GPLv3 license.