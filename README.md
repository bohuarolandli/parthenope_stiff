# PArthENoPEstiff

## New BSM physics

The original PArthENoPE 3.0 code is modified to accommodate new ingredients of Beyond-Standad-Model (BSM) physics, which include:
1. A dark radiation component parametrized by the effective number of relativistic species, **$\Delta N_\mathrm{eff}$**.
2. A stiff component (with equation of state $w=1$) parametrized by its energy density ratio to photons at 10 MeV, **$\kappa_{10}$**.

Some of the key nuclear reaction rates are also updated, which affect the primordial helium and deuterium abundances ($Y_\mathrm{P}$ and D/H).

## Cobaya interface

We provide two interfaces, "par_stiff.py" and "par_stiff_err.py" for Cobaya inference pipelines. Each of the python scripts serves as a theory block.
The errors in **four** key nuclear reaction rates (Nos. 12, 20, 28, 29) are taken as free parameters in "par_stiff_err.py".

## GUI

For the PArthENoPE GUI, we modify the original code so that this version runs on Mac computers with Apple silicon that does not support the original PySide2 package.
Instead, the python codes are modified to allow for an implementation with PySide6 (conda installable).

See the README_parthenope.md file for documatation of the original PArthENoPE 3.0 code.
