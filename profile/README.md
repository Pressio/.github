Pressio is an ecosystem for *developing*, *applying* and *using* projection-based model reduction (pROM) methods. 
A key goal is to mitigate the intrusive nature of pROMs for large-scale codes, and providing a framework to foster research of new ideas and as well as broaded usability. 

Usefule resources: 
- [core C++ library](https://pressio.github.io/pressio/): working towards a production-level ROM capability inevitably means spanning multiple fields ranging from, e.g., linear algebra, nonlinear solvers and optimization, to time integration, distributed computing and HPC. We have been developing this library from the ground up by identifying key building blocks and modularizing them accordingly. The result is a stack of "components" that can be used independently and in a self-contained fashion, but collectively constitute the stack foundation of the ROM capability. Regardless of your interest in ROMs, you might find useful some of the components of the library.

- [demoapps](https://pressio.github.io/pressio-demoapps/): a collection of 1D, 2D and 3D problems of varying complexity (from linear advection, to reaction-diffusion and compressible Euler). It is being developed to be self-contained supporting both C++ and Python interfaces, and with built-in support for samples meshes. You can just use it for doing “standard” simulations, or just use the Python meshing scripts, or leverage the sample mesh capability to study function approximations, or testing the ROM capabilities that pressio provides.

- [tutorials](https://pressio.github.io/pressio-tutorials/): tutorials suite for the pressio C++ library that also leverages pressio-demoapps. 

- [tools and workflows](https://github.com/Pressio): comprises a set of algorithms for constructing and exploiting ROMs that rely on abstract base classes that encapsulate all the information needed to run a given algorithm. 
