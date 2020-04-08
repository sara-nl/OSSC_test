# OSSC_test
Documentation and issue reporting for the OSSC test phase.


## Reporting bugs and issues with the OSSC environment and asking questions
Please report bugs, issues and ask questions to SURF advisors and admins via email to ossc-support@surfsara.nl.

## SLURM usage 
Cartesius uses a job scheduler (SLURM). All the information to get started with SLURM on Cartesius can be found [here (Cartesius user's guide)](https://userinfo.surfsara.nl/systems/cartesius/usage/batch-usage).

## Software environment on Cartesius
The software environment on Cartesius is managed with modules.
More information can be found under [Software environment based on EasyBuild](https://userinfo.surfsara.nl/documentation/new-software-environment-based-easybuild) and [New Module Environment](https://userinfo.surfsara.nl/documentation/new-module-environment-lisa-cartesius).
In the OSSC, the 2019 software stack is loaded by default.

In the OSSC, just as on Cartesius, softwares are managed using modules. Modules provide an easy mechanism for updating a user’s environment, notably the PATH, MANPATH, CPATH, and LD_LIBRARY_PATH environment variables. The advantage of the modules approach is that the user is no longer required to explicitly specify paths for different software versions nor need to try to keep the related environment variables coordinated. With the modules approach, users simply load and unload modules to control their environment.
Users should always choose to use software available in a module rather than the system installation of that software. For example to use python3, load module `Python/3.7.5-foss-2018b` to make the cmmand `python` point to `/sw/arch/RedHatEnterpriseServer7/EB_production/2019/software/Python/3.7.5-foss-2018b/bin/python` rather than `/usr/bin/python`. 


**Remark:** We originally had issues with the module environment in the OSSC due to an incompatibility of the Operating System in the OSSC (CentOS 8) and the software stack that was built in the normal Cartesius environment, which runs RHEL 7. We fixed it by changing to a compatible Operating system in the OSSC (CentOS 7).
# **Warning:** there are incompatibilities between our software stack, which was built on the normal Cartesius environment, and the OSSC environment, which runs a newer version of the Operation System. As a consequence, a large part of the modules are not working as expected. The modules for the GCC compiler are not working on the OSSC environment, please use the OS GCC compiler without loading a module for the moment. 

## Adding documentation
Please add any missing documentation and (non confidential) useful information that may be shared with other users to this github repository, preferably in a separate file.

All feedback is welcome.
