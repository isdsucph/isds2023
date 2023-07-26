# Setup

After installing Miniconda (https://docs.conda.io/en/latest/miniconda.html), you can use the `environment.yml` file in this folder to setup a conda environment with the packages that you will need throughout the course.

1. Add the `environment.yml` file to your course folder and open a terminal there.
2. Run the following command in the terminal: `conda env create -f environment.yml` This will install Python 3.9 and the packages listed in the `environment.yml` file.
3. Run `conda env list` and check whether `isds` is listed. If yes, your installation worked.

From now on, before you run a Python script or open a Jupyter notebook from the terminal, you should first run the command `conda activate isds`. This will ensure that you can use the packages you previously installed.

For more information on how to work with virtual conda environments, check out the excellent documentation (https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) or consult Stack Overflow or the AI tool of your choice.

# Why virtual environments?

The main reason for us is replicability of research. If you want to share your project with others, they can use the same `environment.yml` file to re-create the same conditions on their machine. They should then - in principle - be able to obtain the same results.

The second reason is that you can separately manage different projects that have different software requirements without running into conflicts. For example, one project might work with an older Python version or use different package versions than another. With virtual environments, you simply set up a separate environment with a separate `enviroment.yml` file for each project.