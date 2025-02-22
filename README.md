# README 

`Fermi` is a code made for studying the physical behavour of nuclear reactors and to perform a design of them.

>It solves an eigenvalue problem corresponding to the steady state multigroup diffusion equation, which is an aproximation of the Boltzman Transport Equation. This aproximation is only valid in materials were the relation between absortion and scattering collision of neutrons is small.
>
>Macroscopic cross sections should be provided in order to solve the equations in the domain. They may become from a lattice cell homogenization, and possibly, a condensation to few groups in order to decrease the computational effort.
>
>To perform calculations and solving the problem, `Fermi` take advantage of the finite element method 
to discretize the equations. With this technique, the code is capable of solving the problem over 
unstructured 3d meshes.
>
>The design of `Fermi` was aimed to be a very simple and easy understanding code. The input is a 3d mesh that should be
generated with `gmsh` code and an ASCII file with a particular format which contains information about the cross
sections of each material that exist in the domain. The output can be selected according to the user preferences but the
most used tool is the `VTK` format file which contains the solution of the problem (the spatial distribution of the
scalar flux).

## Installation 

###`PETSC` \& `SLEPc` libraries

Download it from [www.mcs.anl.gov/petsc](www.mcs.anl.gov/petsc) and [http://slepc.upv.es](http://slepc.upv.es). 

###`Fermi`:

```bash
make
```  

## The future  

* Optimization 

* Performance evaluation

* Benchmarking

* Documentation

Guido Giuntoli - [giuntoli1991@gmail.com]

## Extra Notes

For reading this text in a `pdf` format do:
```bash
pandoc README.md -V geometry:margin=.5in --latex-engine=xelatex -o README.pdf
```
