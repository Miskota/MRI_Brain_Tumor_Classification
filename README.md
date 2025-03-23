# MRI Brain Tumor Classification


## Overview
My **semester project** for "Machine Learning" subject.
This project uses Machine Learning techniques to classify brain tumors from MRI scans. I used OpenCV for image processing and preprocessing.
<br><br>

## Classes
- **notumor**
- **glioma** 
- **meningioma** 
- **pituitary**
<br><br>


## Dataset
The dataset is included in this repository as 'agyikepek_4_osztaly'.
<br><br>

## Imports
- OS
- CV2
- Numpy
- Pandas
- Matplotlib
- Scikit-learn
- Seaborn
<br><br>

## Preprocessing Steps
- **Image Clipping**: Removes pixels with lower intensity than the threshold
- **Resize**: Resize to uniform size for the model (Sweet spot around 128x128)
- **Median filter**: For noise reduction and avoiding overfitting
- **Histogram Equalization**: Some of the scans were too dark or bright
- **Flip**: For doubling training data
- **Normalize and Flatten**: Prepare the data for the models
<br><br>

## Training samples
Added the option to disable flipping images belonging to the 'notumor' class to avoid overfitting. 
- **pituitary**: 2688
- **meningioma**: 2678
- **glioma**: 2642
- **notumor**: 1595
<br><br>

## Testing samples
- **pituitary**: 300
- **meningioma**: 306
- **glioma**: 300
- **notumor**: 405
<br><br>

## Models
### RandomForestClassifier
**Overall accuracy**: 0.9661
### LogisticRegression (OneVsRest)
**Overall accuracy**: 0.8902


## Future plans
- Segmentation (U-Net/Watershed)
- Use Deep Learning (CNN, Transfer learning)
