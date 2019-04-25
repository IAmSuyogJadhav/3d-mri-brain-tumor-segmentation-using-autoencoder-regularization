# 3D MRI Brain Tumor Segmentation Using Autoencoder Regularization

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/3d-mri-brain-tumor-segmentation-using/brain-tumor-segmentation-brats-2018)](https://paperswithcode.com/sota/brain-tumor-segmentation-brats-2018?p=3d-mri-brain-tumor-segmentation-using)

![The model architecture](https://www.suyogjadhav.com/images/misc/brats2018_sota_model.png)
<center><b>The Model Architecture</b><br />Source: https://arxiv.org/pdf/1810.11654.pdf</center>
<br />
Implementation of the paper titled 3D MRI brain tumor segmentation using autoencoder regularization by Myronenko (https://arxiv.org/abs/1810.11654). The author (team name: **NVDLMED**) was ranked #1 on the [BRATS 2018](https://www.med.upenn.edu/sbia/brats2018/) leaderboard.

# Progress
Currently, the complete Encoder and the Upper branch of decoder (Ground Truth) have been implemented completely. View the current implementation here: [NVDLMED_Implementation.ipynb](NVDLMED_Implementation.ipynb)

# TODO
- ~Implement the custom loss function that the author used. (L = L<sub>dice</sub> + 0.1 ∗ L<sub>L2</sub> + 0.1 ∗ L<sub>KL</sub> )~ Done!
- Modularize the code and make the model available for customization.

