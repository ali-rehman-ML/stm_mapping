## Spatio-Temporal Mapping

### Install Dependcies

To install the Python bindings, ensure you have the following dependencies:
- PCL (any version 1.8+)
- Eigen3
- pybind11 (`pip3 install pybind11`)
- Python 3.8+ (other versions may work but are untested)

```sh
sudo apt-get update
sudo apt-get install libpcl-dev libeigen3-dev python3-pip
pip3 install pybind11
```
### NDT Registeration Module 

```bash

cd 3rd-party/ndt_omp
sudo python3 setup.py install
```
### GICP Registeration Module 
```bash
cd 3rd-party/fast_gicp
python3 setup.py install --user
```

### Result Visualization

For Visualization install dependencies from [requirements.txt](requirements.txt)

Installing Dependecies in anaconda Environmnet is Recommended. 
Download and Setup [Anaconda](https://www.anaconda.com/download)

#### Setup

```bash
conda create -n stm_env python=3.10
conda activate stm_env
pip install -r requirements.txt

```
#### Run Visualization
- Alignment.
For Allignmnet Visualization , configure Alignment [Config](config/allign_config.yaml)

```bash
python align_vis.py
```

- Growth.
For Growth Visualization , configure Growth Visualization [Config](config/growth_vis.yaml)

```bash
python growth_vis.py
```



