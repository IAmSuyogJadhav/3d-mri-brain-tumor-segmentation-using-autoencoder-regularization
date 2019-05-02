# 3D MRI Brain Tumor Segmentation Using Autoencoder Regularization

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/3d-mri-brain-tumor-segmentation-using/brain-tumor-segmentation-brats-2018)](https://paperswithcode.com/sota/brain-tumor-segmentation-brats-2018?p=3d-mri-brain-tumor-segmentation-using)![https://img.shields.io/badge/Implemented%20in-Keras-red.svg](https://img.shields.io/badge/Implemented in-Keras-red.svg)

![The model architecture](https://www.suyogjadhav.com/images/misc/brats2018_sota_model.png)
<center><b>The Model Architecture</b><br />Source: https://arxiv.org/pdf/1810.11654.pdf</center>
<br /><br />Keras implementation of the paper **3D MRI brain tumor segmentation using autoencoder regularization** by Myronenko A. (https://arxiv.org/abs/1810.11654). The author (team name: **NVDLMED**) ranked #1 on the [BRATS 2018](https://www.med.upenn.edu/sbia/brats2018/) leaderboard using the model described in the paper.

This repository contains the model complete with the loss function, all implemented end-to-end in Keras. The usage is described in the next section.

# Usage
1. Download the file [`model.py`](model.py) and keep in the same folder as your project notebook/script.

2. In your python script, import `build_model` function from `model.py`.

   ```python
   from model import build_model
   ```

   It will download an additional script needed for the implementation, [`group_norm.py`](https://github.com/titu1994/Keras-Group-Normalization/blob/master/group_norm.py), which contains keras implementation for the group normalization layer.

3. Make sure the input MRI scans you are going to feed have <u>channels first</u> format with height, width and depth _all_ divisible by 2<sup>4</sup>, i.e., 16. This is to ensure correct output shape according to the model.

4. Now to create the model, simply run:

   ```python
   model = build_model(input_shape)
   ```

   where, `input_shape` is a 4-tuple (channels, Height, Width, Depth).

# Issues

If you encounter any issue or have a feedback, don't hesitate to [raise an issue](https://github.com/IAmSuyogJadhav/3d-mri-brain-tumor-segmentation-using-autoencoder-regularization/issues/new).