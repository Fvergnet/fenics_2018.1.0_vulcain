# fenics_on_cluster
Scripts to install fenics locally on clusters

## 1. On Vulcain
### Requirements
- Ubuntu 16.04
- The following packages have to be installed with apt-get (by a sudoer) :

  ```
  apt-get update
  apt-get install -y software-properties-common
  add-apt-repository ppa:ubuntu-toolchain-r/test
  apt-get update
  apt-get install -y wget xz-utils build-essential zlib1g-dev checkinstall libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev gfortran libblas-dev liblapack-dev libopenmpi-dev openmpi-bin openssh-client git gcc-6 g++-6
  ```

### Installation
The scripts install 
- dolfin and its dependencies :
```
Python2 and Python3
cmake
Boost
PETSc
SLEPc
EIGEN
Some python modules : matplotlib, numpy, numexpr, ply, six, sympy==1.1.1, pandas, ipython, ipyparallel, h5py, mpi4py, petsc4py, slepc4py, meshio and pygmsh
HDF5
pybind11
fiat
dijitso
ufl
ffc
instant
```
- the remeshing tool `mmg`(www.mmgtools.org)

## 2. Docker container
