Document Sandbox
================================================================================

Development Environment
--------------------------------------------------------------------------------

A few tools are necessary

  - A [LaTeX](https://www.latex-project.org/) distribution,

  - The [git](https://git-scm.com/) version control system,

  - A text editor, file explorer, terminal (bash), etc. 
    or an an IDE like [Visual Studio Code](https://code.visualstudio.com/) 
    that packages these things for you,

  - The [conda](https://conda.io/en/latest/) package & environment manager.

The latter is especially important since we use it to bootstrap 
the installation of many extra software tools that we need,
such as Python, Pandoc, etc. If you don't already have conda on your computer, 
you may install [miniconda](https://docs.conda.io/en/latest/miniconda.html).

Our extra software requirements are listed in the `environment.yml` file.
To create a conda environment that matches this specification, 
once and for all, execute in the terminal:

    $ conda env create -f environment.yml

Now, when you need to work on the project,
activate the environment:

    $ conda activate document-sandbox

Full reference: [Conda/Managing environments](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)


Edit/Build the Document
--------------------------------------------------------------------------------

In the project directory: 

 1. Edit the Markdown version `document.md` of the document,
    its bibliography, etc.

 2. Then, execute the command

        $ ./build

    to create PDF, HTML and ODT versions of the document
    in the `output` directory.