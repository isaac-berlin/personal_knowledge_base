# Python Virtual Enviornments

## Why use them
* makes managing project dependencies eaiser
* prevents conflicts between packages 
* allows better version control for packages

## Installing virtualenv

Make sure you have virtualenv installed
```bash
pip install virtualenv
```

## Windows Setup

```bash
# Create a virtual environment 
python -m venv env_name

# Activate the virtual environment
env_name\Scripts\activate
```

## Linux/Mac Setup

```bash
# Create a virtual environment
python3 -m venv env_name

# Activate the virtual environment
source env_name/bin/activate
```

## Using the virtual environment

```pip install package_name``` - installs a package into the virtual environment

```pip freeze``` - lists all packages installed in the virtual environment

```pip install -r requirements.txt``` - installs all packages listed in the requirements.txt file

```deactivate``` - deactivates the virtual environment

## Using venv with VSCode
* Open the project folder in VSCode
* Open the command palette (Ctrl+Shift+P)
* Type in "Python: Select Interpreter"
* Select the virtual environment you want to use
    * you can navigate to the virtual environment folder
    * select the Scripts/python.exe file
