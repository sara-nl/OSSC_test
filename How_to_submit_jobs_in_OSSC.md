# Job submission within the OSSC

To submit jobs to run on the compute nodes you first need to make a request for a secure virtual cluster. Only when a reservation of a secure virtual cluster is active can you submit jobs to the compute nodes on that cluster.

You can view the slurm logical partitions available to you with the `sinfo` command.
The compute nodes will usually be placed in a partition name `comp_env`.

If no secure virtual cluster is running, as is the case for the first phase of the testing of the OSSC, you can still submit jobs that will run on the work environment.

# SLURM usage
For general guidelines about batch jobs submission with SLURM please refer to the [Cartesius online documentation](https://userinfo.surfsara.nl/systems/cartesius/).

