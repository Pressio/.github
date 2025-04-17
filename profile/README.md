Pressio is an ecosystem for *developing*, *applying* and *using* projection-based model reduction (pROM) methods. 
A key goal is to mitigate the intrusive nature of pROMs and provide a framework to foster research of new ideas as well as incentivize broader adoption and usability. 
We have been developing this ecosystem from the ground up revolving around the following main entities: 

- [pressio-rom](https://github.com/Pressio/pressio-rom): C++ library providing modules for constructing and solving reduced-order models, with or without hyper-reduction. This includes also nonlinear solvers and time integration. Constructing and solving ROM problems can be done ensuring compatibility with various numerical solvers and high-performance computing environments.
This is achieved through the use of generic programming: algorithms are expressed in a flexible, backend- and application-agnostic way.

- [pressio-ops](https://github.com/Pressio/pressio-ops): a lightweight C++ linear algebra library offering a unified interface to a variety of backend libraries—including Eigen, Kokkos, and Trilinos—enabling high-performance, portable computations across different architectures.

- [tools and workflows](https://github.com/Pressio/rom-tools-and-workflows): comprises a set of algorithms for constructing and exploiting ROMs that rely on abstract base classes that encapsulate all the information needed to run a given algorithm. This provides the so-called "outer loop" capabilities for exploiting ROMs, e.g. in UQ. 

- [tutorials](https://pressio.github.io/pressio-tutorials/): tutorials and demos showing how to use the pressio C++ library, and also end-to-end ROMs using pressio-demoapps (we are also working towards integrating the tools-and-workflows library into this).

- [demoapps](https://pressio.github.io/pressio-demoapps/): a collection of 1D, 2D and 3D problems of varying complexity (from linear advection, to reaction-diffusion and compressible Euler). It is being developed to be self-contained supporting both C++ and Python interfaces, exact Jacobians and built-in support for samples meshes. You can just use it for doing “standard” simulations, or just use the Python meshing scripts, or leverage the sample mesh capability to study function approximations, or testing the ROM capabilities that pressio provides.


