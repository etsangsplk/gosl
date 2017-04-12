# Gosl &ndash; Go scientific library

Gosl is a computing library written in go language (golang) to help with the development of software
for scientific research. The library tries to be as general as possible. The use of concurrency for
multi-threaded applications and message passing for parallel computations are considered. Functions
and structures for geometry calculations, random numbers generation and probability distributions,
optimisation algorithms, and plotting and visualisation are implemented as well. This library helped
with the development of the results presented in [1-5].



## Content

1.  chk    &ndash; check and unit test
2.  io     &ndash; input/output
3.  utl    &ndash; utilities
4.  plt    &ndash; plotting
5.  mpi    &ndash; message passing interface
6.  la     &ndash; linear algebra
7.  fdm    &ndash; finite differences method
8.  num    &ndash; numerical methods
9.  fun    &ndash; scalar functions of one scalar and one vector
10. gm     &ndash; geometry
11. gm/msh &ndash; mesh generation
12. gm/tri &ndash; mesh generation: triangles
13. gm/rw  &ndash; mesh generation: read/write
14. graph  &ndash; graph theory
15. ode    &ndash; ordinary differential equations
16. opt    &ndash; optimisation
17. rnd    &ndash; random numbers and probability distributions
18. tsr    &ndash; tensor algebra and definitions for continuum mechanics
19. vtk    &ndash; visualisation tool kit



## Examples

See examples here: https://github.com/cpmech/gosl/blob/master/examples/README.md


<div id="container">
<p><img src="examples/figs/rnd_normalDistribution.png" width="400"></p>
Normally distributed pseudo-random numbers. Using sub-package `rnd`
</div>


## Installation and documentation

1. To install on Windows, [see instructions for Windows here](https://github.com/cpmech/gosl/blob/master/doc/InstallationOnWindows.md)
2. To install on Mac OS X, [see instructions for Mac OS X here](https://github.com/cpmech/gosl/blob/master/doc/InstallationOnMacOSX.md)
3. To install on Debian/Ubuntu/Linux, type the following commands:

```
sudo apt-get install libopenmpi-dev libhwloc-dev libsuitesparse-dev libmumps-dev 
sudo apt-get install gfortran libvtk6-dev python-scipy python-matplotlib dvipng
mkdir -p $GOPATH/src/github.com/cpmech
cd $GOPATH/src/github.com/cpmech
git clone https://github.com/cpmech/gosl.git
cd gosl
./all.bash
```

Make sure that the following environment variable is defined:

```
export PYTHONPATH=$PYTHONPATH:$GOPATH/src/github.com/cpmech/gosl/scripts
```

The documentation for developers is available here: http://rawgit.com/cpmech/gosl/master/doc/index.html






## License

Unless otherwise noted, the Gosl source files are distributed under the BSD-style license found in the LICENSE file.
