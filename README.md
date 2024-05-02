# Driving Drowsiness Detection System

**All the description and guide/pre-request was specified in the jupyter note book.**

## Key things:
- This project was developed under Windows11 Operating System so all the related environment, libraries and dependencies was based on Windows11.

- Since Github have a storage limit, all the dataset files are empty, just for a structure, all the datasets will be on the cloud:
  - If you want to start over (from data pre-processing to the end), your will need to open `Raw data` file from cloud and use `images` and `labels` to replace `data/images` and `data/labels` in the repo.
  - If you want to start from training (all the data already pre-processed), but you want to train the model, you will need to find a file called `Pre-processed data` from cloud, use `data` and `aug_data` in the file to replace the file with same name in repo. After this, locate section 4.4, there will be a check point, run the code blocks from there.
  - If you just want to start use the detection system, a pre-trained model `DualTaskFaceModel.h5` is already in the repo, locate section 10 in the notebook, there will be a check point, run the code blocks from there.
 



### Prepare the environment and pre-request:
**Here recommened to use anaconda environment if you want to use GPU to run tensorflow on windows11.**

Jupyter note book and anaconda3 need to be installed.

`pip install` or `conda install`:
```
numpy
matplotlib
opencv-python 
labelme
albumentations
dilb
pygame
```

**Using anaconda to install CUDA toolkit and cudnn for Tensorflow2.0 and install Tensorflow:**

```
conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
```
Anything above 2.10 is not supported on the GPU on Windows Native
```
python -m pip install "tensorflow<2.11"
```
Verify the installation:
```
python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"
```
(From tensorflow official website)

### Run the code:
Run the code blocks in note book one by one, see "Key things".

## Link to Cloud and little demo video

Cloud: 
https://drive.google.com/drive/folders/1mg3sZ-XKWn5LMOZVHOuB3_AOGgmutiw5

Demo Video: 
https://youtu.be/BjY9PPPNNMw

