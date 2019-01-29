Document Sandbox
================================================================================

Development Environment
--------------------------------------------------------------------------------

A few tools are necessary

  - A [LaTeX](https://www.latex-project.org/) distribution,

  - The [git](https://git-scm.com/) version control system,

  - A text editor or IDE like [Visual Studio Code](https://code.visualstudio.com/),

  - The [conda](https://conda.io/en/latest/) package & environment manager.

The latter is especially important since we use it to bootstrap 
the installation of every other software dependency that we have,
such as Python, Pandoc, etc. If you don't already have `conda` on your computer, 
you may install [miniconda](https://docs.conda.io/en/latest/miniconda.html).

Our extra software requirements are listed in the `environment.yml` file.
To create a conda environment that matches this specification, 
once and for all, execute:

    $ conda env create -f environment.yml

Now, when you need to work on the project,
activate the environment:

    $ conda activate document-sandbox

Full reference: [Conda/Managing environments](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

