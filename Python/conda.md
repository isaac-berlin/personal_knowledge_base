# What is conda?

Conda is an open source package management system and environment management system that runs on Windows, macOS and Linux. Conda easily creates, saves, loads and switches between environments. 

### Why use conda?

* Cross-Platform Compatibility
* Enviornment and Package Management
* Management of Python and Non-Python dependencies

# Using conda

### Installing conda

Download the [Anaconda installer](https://www.anaconda.com/products/individual) for your OS and follow the instructions to install it.

Windows 

* Run the GUI installer
* Open the Anaconda Prompt

Linux/Mac

* Run the bash script and 
* Restart your terminal


### conda commands

```conda create --name env_name``` - creates a new environment named env_name

```conda activate env_name``` - activates the environment named env_name

```conda deactivate``` - deactivates the current environment

```conda env list``` - lists all environments

```conda install package_name``` - installs a package into the current environment

```conda list``` - lists all packages installed in the current environment

```conda install -r requirements.txt``` - installs all packages listed in the requirements.txt file

```conda env export > environment.yml``` - exports the current environment to a file

```conda env create -f environment.yml``` - creates an environment from a file

```conda env remove --name env_name``` - removes an environment

