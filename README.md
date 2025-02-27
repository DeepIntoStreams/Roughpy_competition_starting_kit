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

## Data
For this challenge, the training data is located at [data/ref_data.pkl](data/). This data includes one single path representing the price and volatility processes of a synthetic asset. The path is sampled from `[0, 10]` with `20480` time steps, following the SDE described in competition description. The data is stored in a `.pkl` file and the data shape is `[1, 20480, 3]`.

## Sample submission
We also provide a sample submission bundle at [sample_submission_bundle](sample_submission_bundle/) which includes: 
1) `calibrated_params.pkl`: Dictionary of the calibrated parameters.
2) `model.py`: Script of your model architecture, model loading, and data generation.

Finally, we wish you good luck during the competition and most importantly, have fun!!!
