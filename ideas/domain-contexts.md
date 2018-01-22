# Domain contexts and domain-specific fields

**Project Description**

The original focus of yt was to analyze datasets from astrophysical simulations. However, use of yt has been expanding to other scientific domains, such as nuclear physics, meteorology, and geophysics. Still, much of the infrastructure within yt is built upon the assumption that the datasets being loaded are astrophysical and hydrodynamic in nature. This assumption informs the choice of derived fields made available to the user as well as the default unit system. For example, fields such as “Jeans mass” and “X-ray emissivity” in CGS units are of little use to an earthquake simulation.

The goal of this project is to develop a system for domain contexts, sets of fields and unit systems associated with specific scientific domains. Rather than having all fields be made available to all datasets, each dataset is given a domain context, which specifies the relevant fields and most meaningful unit system. Domain contexts could also be subclassed to provide further specificity, for example, cosmology as a subclass of astrophysics.

**Expected Outcomes**

* Create a data structure to associate with each frontend that enumerates the sets of fields that are relevant to the scientific field of study assocaited with that frontend. Take the field loading machinery, which currently just loops over all sets of fields, and have it only load fields relevant to each frontend.

* With the above as an example, identify and document all of the attributes and functions in user-facing data structures that make sense for astronomical data but not for data from other fields. Use this to come up with a set of attributes that minimally describe a scientific domain, i.e., sets of fields, the conventional unit system in that field, as well as attributes and functions defined on user-facing data structures.

* Write up a yt enhancement proposal ([YTEP](ytep.readthedocs.org)) describing the proposed design and ideas for implementation. Should identify an initial set of domain contexts, sort fields into domain contexts, and sketch how frontends should declare needed domain contexts.

* Create a domain context class with the identified attributes. Implement a Base, astronomy, and possibly a nuclear engineering domain context and associate it with the existing frontends.

**Skills required/preferred**

At least intermediate-level Python experience. Introductory undergraduate level Physics knowledge. More specific domain-specific knowledge of any one of astronomy, hydrodynamics, finite-element methods, GIS, meteorology, geophysics, or oceanography a plus

**Possible Mentors**

* Nathan Goldbaum (primary)
* Matthew Turk

**Difficulty Rating**

Beginner to Intermediate

