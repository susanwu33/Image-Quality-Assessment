# Image-Quality-Assessment
Different models used to do IQA (classification model and multi-task model) 🥳

To do:
- [X] Upload the classification notebook
- [X] Upload the multi-task notebook
- [X] Write up some instructions and explanations
- [ ] More improvements and ideas coming up ... 🧐

## Classification model

**Data preprocessing**
  - Customized dataset class (MyDataset)
  - Customized transform techniques

**Model**
  - Mainly use the pre-trained models from the torchvision
  - Define a train function for the training process

**Visualisation**
  - Implement GradCam to visualize the heat map

## Multi-task model (Classification + Segmentation) 

!! what's new

**Data preprocessing**
  - Customized dataset class (MyDataset) with special techniques to handle both images and masks
  - Mix batch sampler to keep a balanced proportion of each type of images in the same batch (with/without mask)

**Model**
  - Utilize the pre-trained models from the repository segmentation models
  - Define some customized loss functions (Dice loss and Lovasz loss)
  - Define a Sigmoid-like technique to adjust the weight between classification and segmentation loss (so that it can change over epochs!)

**Visualisation**
  - Implement the output of generated mask

## Free thoughts
- Possible implementation to measure uncertainty (e.g. Monte Carlo dropout / majority voting ...?)
