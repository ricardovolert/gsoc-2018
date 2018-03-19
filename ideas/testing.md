# Improve test coverage and test performance

**Project Description**

Currently yt’s test suite is split between unit tests (which take about 45 minutes to run) and answer tests, which are normally only run on a continuous integration server and take a comparable amount of time to run. Altogether, our current estimate is that the tests only cover about a third of the yt codebase, so much of the existing code in yt needs better test coverage. Additionally, the tests take a long time to run, and we would like to reduce the test runtime while simultaneously increasing code coverage.

This project could go in a number of directions:

* Implement a way to retrofit the current tests for different geometries (e.g. Cartesian, cylindrical, and spherical coordinates) and data styles (e.g. particle data, as well as various kind of mesh data, including uniform resolution, octree, patch AMR, and unstructured meshes). Ideally this would allow us to test all functionality for all possible data styles. This will require learning and improving the “Stream” frontend, which allows the ingestion of in-memory data into yt.

* Identify areas of the code that are not well tested and devise tests for them. This will require measuring the test coverage of yt’s Python and Cython components. The student working on this will need to gain familiarity with untested or undertested parts of the codebase and add new tests. Optimally the new tests will make use of new reusable infrastructure that will be helpful for tests across the yt codebase.

* Improve volume rendering and visualization unit tests. Right now visualization tests rely heavily on answer testing and image comparison. It would be more flexible and easier to understand when things go wrong if the tests instead compared with a predicted answer using some sort of simplified geometry or via introspection.


**Expected Outcomes**

* Develop a framework for measuring test coverage in yt’s python and cython components. Triage the reports to look for areas that are user facing and have poor test coverage.

* Develop new infrastructure to improve testing of yt functionality on different data types.

* Make a number of pull requests improving test coverage across the yt codebase.


**Skills required/preferred**

At least intermediate Python.
Familiarity with testing in any language.
Familiarity with the `nose` test framework.
Experience with a compiled language like C, C++, or Cython.

**Possible Mentors**

* Kacper Kowalik
* Nathan Goldbaum
* Colin Marc
* Matt Turk (backup)

**Difficulty Rating**

Beginner to Advanced, depending on where the student takes the project
