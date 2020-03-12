# Enhancement-of-Brain-MRI-Tumor-Segmentation-using-Multimodality-Learning
Brain tumor segmentation of Brats 2019 with Multimodality Learning
# Abstract
Brain MRI tumor segmentation with new approch of fusion of four modalities as given in the Brats 2019 dataset. Fusion of FLAIR,T1,T2,T1CE and calculating the Dice Coefficient of the whole tumor.
# Proposed Method
![FLow](https://github.com/vaibhav253/Enhancement-of-Brain-MRI-Tumor-Segmentation-using-Multimodality-Learning/blob/master/Segmentation%20Flow/Flow%20Diagram.png)

The main porpose is Brain  tumor  MRI segmentation using  U-Net  architecture. As there are four different  modalities  for  the  given  namely,  T1,  T1ce,  T2  and FLAIR modalities. The four modalities are fused in to one input and converted into numpy array. And, Generating the three diffrent label of ground truth namely Whole tumor, Core tumor, and Enhanced tumor with the use of given Ground truth to compate the whole tumor with predicted whole tumor. Fusion of inputs shown in below figure,
![Fusion of Inputs](https://github.com/vaibhav253/Enhancement-of-Brain-MRI-Tumor-Segmentation-using-Multimodality-Learning/blob/master/Segmentation%20Flow/Input%20Fusion.png)
# Data Preprocess
In the data preporcessing, the first step is to resizing the image size 240X240 into 192X192 according the U-Net architecture. The second step is removing the unncessary slices. So removed the first 30 and last 35 slices and selecting only middle 90 slices.
# Dataset
Whole dataset you can download from: [MICCAI 2019](https://www.med.upenn.edu/sbia/brats2018.html)

Download Numpy array of each modalities and Fused Images from: [Data Array](https://drive.google.com/open?id=1OPy6Mk4AVp9B7BIvr7C0h8nTtofd_vF0)

