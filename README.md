Document Sandbox
================================================================================

Development Environment
--------------------------------------------------------------------------------

To simplify the management of software tools required to work on the project,
the [conda](https://conda.io/en/latest/) package & environment manager is used.

If you don't have it already, you may install
[miniconda](https://docs.conda.io/en/latest/miniconda.html).

### Conda Quickstart

**Reference:** [Managing environments](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

The `environment.yml` file lists the project software requirements.
To create a conda environment that matches this specification, execute:

    $ conda env create -f environment.yml

and to activate it:

    $ conda activate document-sandbox

The command prompt now shows that the environment is activated:

    (document-sandbox) $

To get back to normal when you're done working on the project,
deactivate the environment with the command `conda deactivate`.

If your version of the environment is outdated 
(there is a new `environment.yml` file), update it

    $ conda env update -f enviroment.yml

or remove it with `conda env remove --name document-sandbox`
and start over the creation process.

