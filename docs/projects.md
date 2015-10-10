# Projects

## Ongoing

<ul>
  <li>
    <i>femplus</i><br>
    C++ library implementing some algorithms of conventional finite element method (CG), discontinuous Galerkin method (DG) and generalized     multiscale finite element method (GMsFEM), which combines computational algorithms of both CG (on fine scale) and DG (on coarse scale). One of the main features of     this project is that it provides convenient tools to use GMsFEM at work with complicated geometrical characteristics of Earth models. The developement goes in colla    boration with an industrial company sponsoring the project, therefore the code is not open.<br/>
    Keywords: C++, OOD, STL, PETSc, SLEPc, JADAMILU, CMake, Matlab, VTK
  </li>
  <li>
    <i>gmsfem</i><br>
    C++ application running the solution of acoustic and elastic wave equations with Dirichlet and absorbing boundary conditions in domains     with top surface topography using the state-of-the-art GMsFEM. In future, other geometrical features such as caves and fractures are supposed to be incorporated int    o the models. This application completely relies on the <i>femplus</i> library, and it is also not in open access due to proprietary license.<br>
    Keywords: C++, OOD, femplus, Paraview
  </li>
</ul>

## Recent

<ul>
  <li>
    [tethex](http://github.com/martemyev/tethex)
    C++ application converting triangular/tetrahedral meshes into quadrilateral/hexahedral ones. It was implemented mainly to play with     <i>deal.II</i> library. One of the main drawbacks of that library is that it does not support simplicial meshes (i.e. triangular and tetrahedral). And since my PhD     project required a work with complicated geometries, the idea was to try and apply <i>deal.II</i> for those models split on tetrahedra first and then converted to h    exahedrals. Some comparisons were made, after what <i>deal.II</i> and <i>tethex</i> were put aside. However some people found <i>tethex</i> useful for their project    s, and <i>deal.II</i> authors put a note about it on their FAQ page.<br>
    Keywords: C++, Gmsh, deal.II, boost
  </li>
  <li>
    [<i>mixture</i>](http://github.com/martemyev/mixture)
    C++ application for definition of a geometry consisting of a random set of different geometrical shapes inside a cube (can be used t    o define a geometry of a mixture). It was implemented as a part of my PhD project, where I had to model rock samples containing grains of different shape, size, loc    ation and orientation. The resulting geometry is described in <i>Gmsh</i>'s embedded language, which requires the grains not to intersect each other. To avoid this     restriction some successfull attempts to use more sophisticated CAD tools such as <i>OpenCascadeTechnology</i> and <i>FreeCAD</i> have been made, but eventually the    y have not been included into the final version, since the simplest case with bare <i>Gmsh</i> capabilities was found to be sufficient.<br>
    Keywords: C++, Gmsh, OpenCascadeTechnology, FreeCAD, boost
  </li>
</ul>

## Previous

<ul>
  <li>
    <i>Multiscale3D</i><br>
    C++ application performing numerical homogenization of electrical resistivity of rock samples containing grains of different shapes,     size, location and orientation. This is my PhD project, which is not in open access due to its proprietary license belonging to Institute of Petroleum Geology and     Geophysics SB RAS. The project implements parallel algorithms of standard multiscale finite element method for periodic and aperiodic media. Parallel versions are d    eveloped using OpenMP for systems with shared memory, and using MPI for computer clusters. The project was successfully used on two supercomputers: one is in Novosi    birsk State University, another is in Keldysh Institute of Applied Mathematics RAS.<br>
    Keywords: C++, OOD, STL, OpenMP, MPI, Tecplot, mixture
  </li>
  <li>
    [<i>VFEM</i>](./sources/vfem.tar.gz)
    Fortran90 application for solution of Helmholtz equation in 3D. It implements algorithms of vector finite element method (with Nedel    ec basis functions) and two-level solver designed specifically for those basis functions (more details <a href="http://www.sciencedirect.com/science/article/pii/S08    98122107007328">here</a>). This is my M.Sc. project, I don't maintain it, but still keep it.<br>
    Keywords: Fortran90, VFEM, two-level solver, Tecplot
  </li>
</ul>

