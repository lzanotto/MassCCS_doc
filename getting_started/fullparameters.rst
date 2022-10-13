Complete Parameters description 
===============================

Each possible program option that can be used in an input file will be listed in
the following few sections of this manual along with a brief explanation of it's
functionality. It should be noted that not every option is required to be included
in an input file, and the user can choose which (if any) are appropriate for
their calculations. Thus, all options, including the input file itself, is optional.
As a result, each variable that can be changed will also have a default value.

numberProbe-tag
---------------
Default: 1000
number of trajectories calculations per CCS integral.

nIter-tag
---------
Default: 10
number of CCS integrals.

nthreads-tag
------------
Default: maximal available threads
number of threads.

Temp-tag
--------
Default: 298.0 K
Temperature of buffer gas in Kelvin.

seed-tag
--------
random number seed to use for random positions of buffer gas around the target 
molecule and generate their velocities distribution according to the select temperature.

dt-tag
------
Default: 10 fs
time step in fs.

skin-tag
--------
Default: 0.01 Å
skin size of unit cell

GasBuffer-tag
-------------
Default: He
select buffer gas type between He or N2 or CO2.

Equipotential-tag
-----------------
Default: no
Calculation of ellipsoid enveloped around the target molecule to shoot the
buffer gas. Select yes to perform equipotential calculation that is very slowly
for lager sytems (more than 50,000 atoms) or no if applied cutoff radius to
the force calculations.

Short-range cutoff-tag
----------------------
Default: yes
select yes to applied cutoff to Lennard-Jones force or no to otherwise.

LJ-cutoff-tag
-------------
Default: 10.0 Å
radius cutoff of Lennard-Jones force.

Long-range forces-tag
---------------------
Default: no
select yes to applied long-range forces or no to otherwise.

Long-range cutoff-tag
---------------------
Default: no
select yes to applied cutoff to long-range forces or no to otherwise.

Coul-cutoff-tag
---------------
Default: 20.0 Å
radius cutoff of long-range force.

polarizabilty-tag
-----------------
Default: no
select yes to applied induce dipole interactions or no to otherwise.

.. warning:: 
    MassCCS can also handle other linear buffer molecules like CO2, although the 
    interaction parameters have not been parameterized for CCS calculations using carbon dioxide.