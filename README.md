# Learning and Reproduction of Gestures by Gmitation

An implementation of the paper [Learning and Reproduction of Gestures by imitation](https://www.idiap.ch/~scalinon/papers/Calinon-RAM2010.pdf)  from Calinon et al. 
The algorithm proposed in the paper is tested on the Baxter Robot using [rai](https://github.com/MarcToussaint/rai) for control.

The presentation and the code is located in [this](slides/slides_clean.ipynb) jupyter notebook.

## Setup

Running the notebook needs a few initial steps to set up all dependencies. First, install ROS melodic: http://wiki.ros.org/melodic/Installation/Ubuntu

Initialize and clone submodules:

```
git submodule init
git submodule update
```

Download and compile baxter source files:
```
cd external/
./installBaxterSources.sh
cd ..
```

Install additional ubuntu packages needed for rai compilation:
```
make installUbuntuAll
```

Compile rai: 
```
make
```

## Running

Just run
```
jupyter notebook
```
from the repo's root directory.
