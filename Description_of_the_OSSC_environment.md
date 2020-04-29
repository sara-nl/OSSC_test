# Description of the environment
The OSSC consists of a secure work environment and secure virtual cluster.

**The secure work environment** is available for the whole duration of the project, and consists of 4 cores of a Cartesius service node.
It is meant primarily for job preparation, compilation of software, light input preparation and analysis.

**The secure virtual clusters** can be requested by a user following the "secure virtual cluster request procedure". The user can reserve compute nodes (any type of compute node available on Cartesius) for a minimum of 1 day up to maximum 5 days.
Only when the reservation is active can the user access the compute nodes from within the work environment and submit jobs.

**The filesystem** in the OSSC differs from the normal Cartesius filesystem:
- From the OSSC it is not possible to access the shared scratch space for security reasons.
- Home directories on the OSSC are mounted on the Lustre file system, so they can meet the I/O demands of parallel jobs.

As a consequence there is not benefit of using a dedicated `TMPDIR` that would reside on the same file system, and the `TMPDIR` environment variable is left undefined in the OSSC.
If needed, users can create their own user-managed temporary directory, e.g. in `$HOME/tmp`, and define `TMPDIR` in their `.bashrc`.
