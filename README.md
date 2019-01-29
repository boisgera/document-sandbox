Document Sandbox
================================================================================

Development Environment
--------------------------------------------------------------------------------



https://git-scm.com/

Since ... all the tooling required to 

[conda](https://conda.io/en/latest/)

[Managing environments]
(https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

    $ conda env create -f environment.yml
    $ conda activate document-sandbox

The command prompt shows that the environment is activated:

    (document-sandbox) $

To get back to normal when you're done working on the project,
deactivate the environment:

    (document-sandbox) $ conda deactivate

If the `environment.yml` gets updated with new dependencies 
and your version of the environment is outdate, you can update it

    $ conda env update -f enviroment.yml

or remove the environment with `conda env remove --name document-sandbox`
and start over.

