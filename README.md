# Autonomous Driving


## Dependencies

You can install all dependencies by running one of the following command. Recommended!

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

Or you can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.
I've found issues using python 3.7... I recommend sticking to any 3.5 or 3.6


## Usage


### Run the pretrained model

Start up [the Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim), choose a scene and press the Autonomous Mode button.  Then, run the model as follows:

```python
python drive.py model.h5
```

### To train the model

You'll need the data folder which contains the training images.

```python
python model.py
```

This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-001.h5`.

## Credits

The credits go to  [naokishibuya and Siraj Raval] (without whom my academic project would be incomplete)


