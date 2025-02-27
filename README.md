# RoughPy_competition
Welcome to the RoughPy competition!

In this repository, we provide a standard pipeline to help you with the kick-off of our hackathon, the repository contains:
1) Data for training: long_s_path.pkl
2) An illustrative notebook for the RoughPy package
3) A sample calibration method using signatory

## Environment Setup
The code has been tested successfully using Python 3.8 and pytorch 1.11.0. A typical process for installing the package dependencies involves creating a new Python virtual environment.

To install the required packages, run the following:
```
conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=10.2 -c pytorch
pip install signatory==1.2.6.1.9.0 --no-cache-dir --force-reinstall
pip install cupy-cuda102
pip install -r requirements.txt
```
