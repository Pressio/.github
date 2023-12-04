Pressio is an ecosystem for *developing*, *applying* and *using* projection-based model reduction (pROM) methods. 
A key goal is to mitigate the intrusive nature of pROMs for large-scale codes, and providing a framework to foster research of new ideas and as well as incentivize broader adoption and usability. 
We have been developing this ecosystem from the ground up and currently it encompasses the following main entities: 

- [core C++ library](https://pressio.github.io/pressio/): includes several "modules" providing specific capabilities (e.g., on-node and distributed linear algebra kernels, nonlinear solvers and optimization, time integration) that can be used independently and in a self-contained fashion, but collectively constitute the stack foundation of the ROM capability. Regardless of your interest in ROMs, you might find useful some of the components of the library.

- [demoapps](https://pressio.github.io/pressio-demoapps/): a collection of 1D, 2D and 3D problems of varying complexity (from linear advection, to reaction-diffusion and compressible Euler). It is being developed to be self-contained supporting both C++ and Python interfaces, exact Jacobians and built-in support for samples meshes. You can just use it for doing “standard” simulations, or just use the Python meshing scripts, or leverage the sample mesh capability to study function approximations, or testing the ROM capabilities that pressio provides.

- [tools and workflows](https://github.com/Pressio): comprises a set of algorithms for constructing and exploiting ROMs that rely on abstract base classes that encapsulate all the information needed to run a given algorithm. This provides the so-called "outer loop" capabilities for exploiting ROMs, e.g. in UQ. 

- [tutorials](https://pressio.github.io/pressio-tutorials/): tutorials and demos showing how to use the pressio C++ library, and also end-to-end ROMs using pressio-demoapps (we are also working towards integrating the tools-and-workflows library into this).


