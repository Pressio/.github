Pressio is an ecosystem for *developing*, *applying* and *using* projection-based model reduction (pROM) methods. 
A key goal is to mitigate the intrusive nature of pROMs and provide a framework to foster research of new ideas as well as incentivize broader adoption and usability. 
Developed from the ground up, it revolves around the following libraries: 

- [pressio-log](https://github.com/Pressio/pressio-log): Header-only logging utility for the Pressio C++ libraries.

- [pressio-ops](https://github.com/Pressio/pressio-ops): a lightweight C++ linear algebra library offering a unified interface to a variety of backend libraries—including Eigen, Kokkos, and Trilinos—enabling high-performance, portable computations across different architectures.

- [pressio-rom](https://github.com/Pressio/pressio-rom): a C++ library for constructing and solving reduced-order models (ROMs), with or without hyper-reduction. It also includes modular components for time integration and nonlinear solvers. Through the adoption of generic programming and well-defined interfaces, the library is agnostic to the underlying application and data types, enabling seamless integration with diverse numerical solvers and HPC environments.

- [rom-tools and workflows](https://github.com/Pressio/rom-tools-and-workflows): a Python library comprising a set of algorithms for constructing and exploiting ROMs that rely on abstract base classes that encapsulate all the information needed to run a given algorithm. This provides the so-called "outer loop" capabilities for exploiting ROMs, e.g. in UQ. 

- [pressio-tutorials](https://pressio.github.io/pressio-tutorials/): demos showing end-to-end ROMs using pressio-demoapps.

- [pressio-demoapps](https://pressio.github.io/pressio-demoapps/): a collection of 1D, 2D and 3D problems of varying complexity (from linear advection, to reaction-diffusion and compressible Euler). It is being developed to support both C++ and Python interfaces, exact Jacobians and built-in support for samples meshes. You can just use it for doing “standard” simulations, or just use the Python meshing scripts, or leverage the sample mesh capability to study function approximations, or testing the ROM capabilities that pressio provides.

- [pressio-schwarz](https://github.com/Pressio/pressio-schwarz): implements Schwarz coupling for projection-based ROMs with Pressio leveraging some of the apps in pressio-demoapps.

