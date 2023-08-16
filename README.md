# Image-Quality-Assessment
Different models used to do IQA (classification model and multi-task model) 🥳

To do:
- [ ] Upload the classification notebook
- [ ] Upload the multi-task notebook
- [ ] Write up some instructions and explanations
- [ ] More improvements and ideas coming up ... 🧐

## Multi-task model (Classification + Segmentation) 

1. Data preprocessing
  - Customized dataset class (MyDataset)
  - Customized transform techniques

2. Model
  - Mainly use the pre-trained models from the repository segmentation models
  - Define some customized loss functions (Dice loss and Lovasz loss)
  - Define a train function for the training process

3. Visualisation
  - Implement the output of generated mask
  - Implement GradCam to visualize the heat map
