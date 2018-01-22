# Interpolating particle data onto grids

**Project Description**

This project will expand the capabilities of yt to work with data produced by N-body hydrodynamics simulations. Data produced by these simulations consist of a number of volume-filling fields that are defined at the locations of particles. Using a smoothing technique, an interested student will add the ability to interpolate data defined at the locations of particles onto various kinds of meshes.

**Expected Outcomes**

Minimum deliverables:

* An interface to calculate the value of interpolated particle field at an arbitrary location using either the "scatter" or "gather" approach.
* The ability to interpolate particle data onto a uniform resolution mesh

Optional deliverables:

* The ability to interpolate particle data onto an octree mesh.
* An interface to calculate spatial derivatives of a particle field.

**Skills required/preferred**

Programming Languages:

* At least intermediate-level Python experience
* Some experience with C, C++, or another compiled language.

Tools and other skills

* Git and GitHub
* Ability to work with a large python codebase
* Clear communication

Not necessary but would be helpful

* Experience with Cython
* Familiarity with smoothed particle hydrodynamics
* Experience with cluster computing and an MPI libary or an MPI-parallelized simulation code

**Possible Mentors**

* Nathan Goldbaum (primary)
* Meagan Lang (backup)
* Matt Turk (backup)

**Difficulty Rating**

Medium. Much of the infrastructure necessary to implement this deliverables
for this project has already been written. It will be up to the student to
make use of these tools to ensure the project deliverables are finished on-time.

