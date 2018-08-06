# [dl_docker](https://hub.docker.com/r/sysfail/dl_docker/)
## Purpose
Analysis and handling of automotive data with deep learning frameworks. So far without GPU support since it is made to be used on laptops without dedicated Nvidia GPU. (For people who work on the move)
## What is this?
Dockerfile with:
  - Python
    - python 3.6
    - jupyter notebook
  - Data Science Tools
    - [numpy](https://github.com/numpy/numpy)
    - [pandas](https://pandas.pydata.org/)
    - [seaborn](https://seaborn.pydata.org/)
    - [matplotlib](https://matplotlib.org/)
    - [opencv](https://opencv.org/)
    - others like [scipy](https://github.com/scipy/scipy), [plotutils](https://www.gnu.org/software/plotutils/), [pillow](https://pillow.readthedocs.io/en/5.2.x/) etc.
  - Deep Learning Frameworks
    - [Tensorflow 1.8](https://github.com/tensorflow/tensorflow)
    - [Keras 2.2](https://keras.io/)
    - other DL utilities like [tflearn](https://github.com/tflearn/tflearn), [gym](https://github.com/openai/gym), [scikit-learn](https://github.com/scikit-learn/scikit-learn) etc.
  - Libs and Tools to tinker with automotive stuff
    - [ptyhon-can](https://github.com/hardbyte/python-can) to handle raw CAN data (blf, asc)
    - [mdfreader](https://github.com/ratal/mdfreader) to hanle mdf logs
    - [asammdf](http://asammdf.readthedocs.io/) to handle mdf and CAN logging
    - [canmatrix](https://github.com/ebroecker/canmatrix) to handle and convert dbc files
    - [can-utils](https://github.com/linux-can/can-utils) userspace utilities for SocketCAN
    - [pyvit](https://github.com/linklayer/pyvit) Framework to easily work with CAN interfaces and SocketCAN
  - Some examples and tutorials for
    - Tensorflow
    - Keras
    - Python data handling
## How to use
### Build yourself
1. Make sure you have docker installed
2. run *build_docker.sh*
3. run *run_docker.sh*
  - it will start *sysfail/dl_docker*
  - it will link the folder *~/docker/share* (where you should store the files you want to work with)
  - it will expose port 8888 (jupyter notebook) and 6006 (tensorboard)
  - it will open the a browser tab pointing to http://localhost:88888
### Run the pre-build docker
1. Make sure you have docker installed
2. run *run_docker.sh*
  - it will download *sysfail/dl_docker* from [Docker Hub](https://hub.docker.com/r/sysfail/dl_docker/)
  - rest see above ...

### Supported systems
Tested on:
- Ubuntu 16.04 LTS and Docker 18.05
- Ubuntu 18.04 LTS and Docker 18.05
- Ubuntu 18.04.1 LTS and Docker 18.06
- Mac OS Sierra (10.12.6) and Docker 18.03

| **Be aware that due to convenience the jupyter is running without a password or token!** |
|------------------------------------------------------------------------------------------|
