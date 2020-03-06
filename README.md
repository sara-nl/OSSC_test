# OSSC_test
Documentation and issue reporting for the OSSC test phase.


## Reporting bugs and issues with the OSSC environment and asking questions
Please report bugs, issues and ask questions to SURF advisors and admins via email to ossc-support@surfsara.nl.

## SLURM usage 
Cartesius uses a job scheduler (SLURM). All the information to get started with SLURM on Cartesius can be found [here (Cartesius user's guide)](https://userinfo.surfsara.nl/systems/cartesius/usage/batch-usage).

## Software environment on Cartesius
The software environment on Cartesius is managed with modules.
More information can be found under [Software environment based on EasyBuild](https://userinfo.surfsara.nl/documentation/new-software-environment-based-easybuild) and [New Module Environment](https://userinfo.surfsara.nl/documentation/new-module-environment-lisa-cartesius).

**Warning:** there are incompatibilities between our software stack, which was built on the normal Cartesius environment, and the OSSC environment, which runs a newer version of the Operation System. As a consequence, a large part of the modules are not working as expected. The modules for the GCC compiler are not working on the OSSC environment, please use the OS GCC compiler without loading a module for the moment. 

## Adding documentation
Please add any missing documentation and (non confidential) useful information that may be shared with other users to this github repository, preferably in a separate file.

All feedback is welcome.
