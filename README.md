# AI-based HER2 Scoring for Breast Cancer Diagnosis

This repository contains the code and saved models of my thesis project on improving the accuracy and efficiency of diagnosing human epidermal growth factor receptor 2 (HER2) status in breast cancer patients using artificial intelligence and machine learning.

## Thesis
The thesis can be read using the following link: https://drive.google.com/file/d/1W0hDBG_E-ck_FRWe8vkC1UU2Wr3mq5AB/view?usp=sharing

## Abstract

Breast cancer still remains at the top among all the cancers that affect women across the globe. Early detection by accurate diagnosis is the key to successful treatment and to increasing survival. Despite the diagnostic methods used being effective, they have some limitations because of the variability in the outcome due to human error and subjectivity. HER2 is a protein whose overexpression relates to more aggressive types of breast cancer and less favorable prognoses. Accurate HER2 status assessment is crucial in guiding treatment decisions, especially with the advent of targeted treatment approaches, such as Trastuzumab (Herceptin). Traditional assessment of HER2 status has been done through Immunohistochemistry (IHC) and Fluorescence In Situ Hybridization (FISH), both of which have a high degree of variability and require extended time and pathologist expertise. The purpose of this dissertation is to explore the application of artificial intelligence and machine learning to improve the accuracy and efficiency of diagnosing human epidermal growth factor receptor 2 (HER2) status for breast cancer patients. Moreover, in this research, the utility of Hematoxylin & Eosin (H&E) stainings for AI-driven HER2 scoring is analyzed. An empirical study using a public dataset testing several deep learning approaches and techniques to establish the performances of AI in HER2 scoring has been conducted in this project. It explored data augmentation and training techniques, including undersampling, oversampling, weight decay, and class weight adjustments, to tackle class imbalance and overfitting in HER2 classification. Batch sizes and learning rates have been explored to find the best combination. Image preprocessing included a comparison of RGB and Grayscale color spaces and a size comparison between 224x224 and 448x224 image formats. Additionally, Grad-CAM was used to identify regions of pathology images that the CNN focused on, enhancing the interpretability of the model’s predictions. After finding the best parameters and preprocessing approach, the final model (ResNet18) reached 94% accuracy on the test set in less than 100 epochs. H&E stainings resulted to be useful to enhance the model’s performance. RGB and 224x224, respectively, color space and input image format were the best choices for this task. A learning rate of 0.001 and batch size of 256 resulted to be the most effective. The Grad-CAM results achieved suggest promising future work for a better understanding of CNNs in HER2 scoring.


## Conclusion

This research aimed to find solutions to all the issues of HER2 scoring for breast cancer tissues using machine learning methods. The main goal was to enhance the accuracy, consistency, and efficiency of HER2 scoring by leveraging convolutional neural networks (CNNs) for image analysis. The final model obtained an accuracy of 94% on the unseen data, an excellent result for relatively small training data. The best combination found was with a batch size of 256 and a learning rate of 0.001. Depending on the case, 75 to 100 training epochs were used, and both were more than enough to let the model be well trained. The present study confirmed that
adding Hematoxylin and Eosin images to Immunohistochemistry images improved the model’s predictive power with respect to the HER2 status. The performance of the integrated approach was higher than that of models based on just H&E or IHC images, indicating the synergistic value brought by having two imaging modalities.

Various data augmentation and sensitive training techniques, such as undersampling, over- sampling, weight decay and class weight, were explored to address class imbalance and over- fitting. They probably didn’t improve the performances because the dataset was too small, and those approaches were not enough to enhance the model’s accuracy. Different image pre-processing were compared. The results showed that RGB colour space performs better than Grayscale. The size of the input concatenated images was also explored, and the 224x224 format performed better than the 448x224 format. The latter was used to see if maintaining the original images’ ratio could help the accuracy rate. On the contrary, this gave slightly worse results, meaning 224x224 input images are the most effective.
The implementation of Gradient-weighted Class Activation Mapping (Grad-CAM) provided valuable insights into the regions of pathology images that the CNN focused on for HER2 classification.

## Repository Contents

- **Code**: In the repository are available some of the Jupiter notebooks that i'm working on.



