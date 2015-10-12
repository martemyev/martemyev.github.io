# Projects

## Ongoing

* _femplus_<br/>
  C++ library implementing some algorithms of conventional finite element method (CG), discontinuous Galerkin method (DG) and generalized multiscale finite element method (GMsFEM), which combines computational algorithms of both CG (on fine scale) and DG (on coarse scale). One of the main features of this project is that it provides convenient tools to use GMsFEM at work with complicated geometrical characteristics of Earth models. The developement goes in collaboration with an industrial company sponsoring the project, therefore the code is not open.<br/>
  Keywords: C++, OOD, STL, PETSc, SLEPc, JADAMILU, CMake, Matlab, VTK

* _gmsfem_<br/>
  C++ application running the solution of acoustic and elastic wave equations with Dirichlet and absorbing boundary conditions in domains with top surface topography using the state-of-the-art GMsFEM. In future, other geometrical features such as caves and fractures are supposed to be incorporated into the models. This application completely relies on the <i>femplus</i> library, and it is also not in open access due to proprietary license.<br/>
  Keywords: C++, OOD, femplus, Paraview

## Recent

* [_tethex_](http://github.com/martemyev/tethex)<br/>
  C++ application converting triangular/tetrahedral meshes into quadrilateral/hexahedral ones. It was implemented mainly to play with _deal.II_ library. One of the main drawbacks of that library is that it does not support simplicial meshes (i.e. triangular and tetrahedral). And since my PhD project required a work with complicated geometries, the idea was to try and apply _deal.II_ for those models split on tetrahedra first and then converted to hexahedrals. Some comparisons were made, after what _deal.II_ and _tethex_ were put aside. However some people found _tethex_ useful for their projects, and _deal.II_ authors put a note about it on their FAQ page.<br/>
  Keywords: C++, Gmsh, deal.II, boost

* [_mixture_](http://github.com/martemyev/mixture)<br/>
  C++ application for definition of a geometry consisting of a random set of different geometrical shapes inside a cube (can be used to define a geometry of a mixture). It was implemented as a part of my PhD project, where I had to model rock samples containing grains of different shape, size, location and orientation. The resulting geometry is described in _Gmsh_'s embedded language, which requires the grains not to intersect each other. To avoid this restriction some successfull attempts to use more sophisticated CAD tools such as _OpenCascadeTechnology_ and _FreeCAD_ have been made, but eventually they have not been included into the final version, since the simplest case with bare _Gmsh_ capabilities was found to be sufficient.<br/>
  Keywords: C++, Gmsh, OpenCascadeTechnology, FreeCAD, boost

## Previous

* _Multiscale3D_<br/>
  C++ application performing numerical homogenization of electrical resistivity of rock samples containing grains of different shapes, size, location and orientation. This is my PhD project, which is not in open access due to its proprietary license belonging to Institute of Petroleum Geology and Geophysics SB RAS. The project implements parallel algorithms of standard multiscale finite element method for periodic and aperiodic media. Parallel versions are developed using OpenMP for systems with shared memory, and using MPI for computer clusters. The project was successfully used on two supercomputers: one is in Novosibirsk State University, another is in Keldysh Institute of Applied Mathematics RAS.<br/>
  Keywords: C++, OOD, STL, OpenMP, MPI, Tecplot, mixture

* [_VFEM_](../for_homepage/sources/vfem.tar.gz)<br/>
  Fortran90 application for solution of Helmholtz equation in 3D. It implements algorithms of vector finite element method (with Nedelec basis functions) and two-level solver designed specifically for those basis functions (more details [here](http://www.sciencedirect.com/science/article/pii/S0898122107007328)). This is my M.Sc. project, I don't maintain it, but still keep it.<br/>
  Keywords: Fortran90, VFEM, two-level solver, Tecplot
