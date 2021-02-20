# Night-to-Day-Image-Translation-using-DCGAN

An supervised night to day image translation using **Deep Convolutional Generative Adversarial Network**

## Prerequisites
- Python 3
- Tensorflow
- CPU or NVIDIA GPU + CUDA CuDNN

## Instalation

### Clone this repo
```
  git clone https://github.com/evanezcent/Night-to-Day-Image-Translation-using-DCGAN/
```

### Install
```
  pip install tensorflow
  pip install PIL
  pip install pydotplus
  pip install IPython
  pip install numpy
  pip install pandas
```

## Dataset
We provided our augmented [dataset](https://drive.google.com/drive/folders/1W0DIj-2M-BCVi4FfPsl_zYhNS304Uh1K?usp=sharing) and [datatest](https://drive.google.com/drive/folders/1sSjqPcK8IYGJ0Rx9qWJs0QX3Sgry6KS4?usp=sharing) which has a square shape. If you want the un-augmented data, just email me [here](pratamayo16@gmail.com)

## Data Preparation
On data preparation, we extract many timelapse video and then tak 5~10 copies of the image.

## Data Augmentation
We just doing two kind of augmentation process, that is cropping and flipping to keep the original feature of the images. Then we renamed it sequentially.

## Testing
We evaluate the model using `SSIM` as the `accuracy` and `L2-Norm` to calculate the `loss`.

## Result
As the final result, we just get a `40% accuracy` using datatest. Based on our analytics, it caused of :
  - Lack of paired image data night and day
  - Training time
  - Suitable architecture for night to day translation case

### Using testing images
<img src="/final-model-test.png" width="700">

### Using training images
<img src="/final-model-train.png" width="700"> 

## Paper
**SOON**
