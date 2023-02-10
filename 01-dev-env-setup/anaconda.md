 # Anaconda
 
 <img src="../assets/images/anaconda_logo.png" style="width:50;"/>
 
 [Anaconda](https://www.anaconda.com/) is a very popular python distribution and development environment.
 
 Follow the [install guide](https://www.anaconda.com/products/distribution) and setup anaconda on your machine.
 
 **Do I need anaconda even if my system has Python installed?**
 
 Yes.  Because system python's can be different versions.  And we don't recommend upgrading system python packages, as it may mess up with system functions
 
 Anaconda installs in 'user-space' in it's own directory.  Doesn't interfere with system python packages.  And behaves very well.
 
 ## Setting up an Anaconda Environment
 
 When you install Anaconda, it creates a 'base' environment.  This one, as you might guess, has all the basic necessities to get anaconda running.
 
 Anaconda supports different environments that are isolated for different projects.
 
**It is highly recommended to setup dedicated environments for projects**


### Option-1: Create an env manually


This instructions for using conda command line 


```bash
$   conda env list

$   conda create --name pyds python

$  conda activate pyds
# make sure your prompt says "pyds"

# install any extra packages by
$   conda install  numpy pandas seaborn scikit-learn  jupyterlab

# verify packages by 
$   conda list

# start jupyter
$   jupyter lab
```

### Option 2 : Create Using YML file

Inspect this file [pyds.yml](pyds.yaml)

This file defines environment configuration

Install as follows

```bash
$   conda env create -f pyds.yaml

$   conda env list
```

To access the environment, activate it

```bash
$   conda activate  pyds
```

To end the environment, deactivate it

```bash
$   conda deactivate
```

To remove any conda environment

```bash
$   conda deactivate pyds

$   conda env remove -n pyds
```