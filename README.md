<h1 align="center">
Age-Detection-Facial-Images
</h1>  

## Project Overview

The Age Detection project aims to classify the age of individuals from facial images using deep learning techniques. The primary goal was to design and deploy a model capable of accurately predicting the age range of individuals based on their facial features.

## Dataset

The project utilized the Kaggle Facial Image Dataset, which includes three age categories: Young, Middle, and Old. The dataset consists of 19,906 facial images, each associated with an age label. These categories allowed for a more detailed analysis of age prediction.

## Approach
1. **Data Preprocessing:** To enhance model performance, various preprocessing techniques were applied to the images. This included image resizing, denoising, and normalization. Furthermore, categorical encoding was performed to represent age categories numerically.

2. **GPU Utilization:** The power of GPU was harnessed for faster model training. This significantly reduced training time and allowed for experimentation with different architectures and hyperparameters.

3. **Data Analysis:** Class visualization techniques were employed to better understand the distribution of age categories within the dataset. The analysis revealed a class imbalance issue, which could affect model performance.

4. **Data Augmentation:** To mitigate the class imbalance, data augmentation techniques such as RandomFlip and RandomRotation were applied. These techniques artificially increased the diversity of the dataset, aiding the model in learning from a more balanced representation of age categories.

5. **Model Architecture:** Two different approaches were taken for model building and training:

    a. Deep CNN Model: A custom deep convolutional neural network was designed from scratch. The architecture was tailored to the specifics of age detection from facial features.

    b. Fine-tuning VGG16 Model: A pre-trained VGG16 model was utilized as a base. The model was fine-tuned on the dataset to adapt it for age detection. This approach leveraged transfer learning         for enhanced accuracy.


## Results

The Age Detection model achieved a promising accuracy rate of 84% using the custom Deep CNN model and 72% using the fine-tuned pre-trained VGG16 model. The application of data augmentation techniques further improved the model's performance by addressing the initial class imbalance issue.

## Future Enhancements

This project lays the foundation for further improvements in age detection accuracy. Future enhancements may include exploring different architectures, incorporating advanced preprocessing techniques, implementing ensemble methods, and fine-tuning the data augmentation strategies.
