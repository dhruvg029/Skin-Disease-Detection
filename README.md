# Skin Disease Detection with Saliency Maps
This is the boilerplate code for skin disease detection with the help of U-Net Segmentation and showcasing the visualization with the help of Saliency Maps. 

## Introduction
This is the basic code for the [CVIP 2022](https://link.springer.com/chapter/10.1007/978-3-031-31407-0_25) article. A model is proposed which uses an image set that is pre-processed by various techniques like deblurring, noise reduction, and then enhanced. The images are then segmented using U-Net and MobileNetV2 is used for classification. 

## Results
<p align="center">
<img src="https://github.com/dhruvg029/Skin-Disease-Detection/blob/main/SkinDiseaseDetection/download.png", width="720">
</p>

## Datasets
**1. PH2 dataset:** Contains a total of 200 dermoscopic images of melanocytic lesions, including 80 common nevi, 80 atypical nevi, and 40 melanomas. The dataset can be accessed from [here](https://www.fc.up.pt/addi/ph2%20database.html).
<p align="center">
<img src="https://github.com/dhruvg029/Skin-Disease-Detection/blob/main/SkinDiseaseDetection/ph2.png", width="250" height="250">
</p>

**2. HAM10000 dataset:** Consists of 10015 dermatoscopic images and is a representative collection of all important diagnostic categories in the realm of pigmented lesions. The dataset can be accessed from [here](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T).
<p align="center">
<img src="https://github.com/dhruvg029/Skin-Disease-Detection/blob/main/SkinDiseaseDetection/ham10000.png", width="300">
</p>

## Testing Steps
1. Make sure your datasets are loaded correctly.
2. After loading your datasets, run `UNET_SEGMENATION.ipynb` to get the segmented images after processing.
3. Run those segmented and augmented images with `MobileNetV2.ipynb` for classification.
4. Run `SaliencyMap.ipynb` to visualization the images with the help of saliency maps.
   
## Citation
Please cite the paper in your publications if it helps your research:  

    @InProceedings{10.1007/978-3-031-31407-0_25,
      author="Toteja, Rishit
      and Gupta, Dhruv
      and Gautam, Vibhor
      and Vishwakarma, Dinesh Kumar",
      title="Skin Disease Detection Using Saliency Maps and Segmentation Techniques",
      booktitle="Computer Vision and Image Processing",
      year="2023",
    }
