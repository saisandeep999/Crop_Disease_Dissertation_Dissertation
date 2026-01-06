# Crop_Disease
# Introduction

This project focused on the comparative evaluation of machine learning techniques for predicting crop diseases using environmental and image data. Crop diseases are a major threat to agricultural productivity, food security, and farmers’ livelihoods worldwide. Traditional disease detection approaches, such as manual inspection and laboratory testing, are often slow, costly, and difficult to scale across large agricultural fields. These limitations highlight the need for automated, data-driven solutions capable of providing early and accurate disease identification.

To address this challenge, this study adopted a multimodal machine learning approach by integrating visual features extracted from plant leaf images with environmental factors such as temperature and humidity. By combining symptom-based image analysis with causal environmental indicators, the project aimed to build more robust and realistic disease prediction models suitable for smart agriculture applications.

# Dataset Description and Link

The primary dataset used in this study was the PlantVillage dataset, a widely recognised benchmark dataset for plant disease classification. It contains over 50,000 high-quality RGB images of healthy and diseased plant leaves across multiple crop species and disease categories. The dataset is well-labelled, balanced, and suitable for supervised learning tasks.

Dataset name: PlantVillage

Image type: RGB leaf images

Number of disease classes: 38 (healthy and diseased)

# Dataset link:
https://data.mendeley.com/datasets/tywbtsjrjv/1

Since the PlantVillage dataset does not include real environmental data, synthetic and supplementary environmental variables (such as temperature and humidity) were incorporated based on agricultural and meteorological references to simulate realistic disease development conditions.

# Techniques Applied

The project followed a quantitative, experimental, and comparative research design. The main techniques applied include:

Image preprocessing: resizing, normalization, noise reduction, contrast enhancement, and data augmentation.

Feature engineering: extraction of colour (RGB and HSV histograms), texture, and statistical features from images, combined with environmental variables to form a multimodal feature vector.

Machine learning models implemented:

Support Vector Machine (SVM)

Random Forest (RF)

Logistic Regression (LR)

K-Nearest Neighbours (KNN)

Model evaluation techniques:

Train–test split (80:20)

10-fold cross-validation

Performance metrics: Accuracy, Precision, Recall, F1-score, and AUC-ROC

All models were trained using identical datasets, preprocessing pipelines, and evaluation strategies to ensure a fair comparison.

# Results

The experimental results demonstrated clear performance differences among the evaluated models. Support Vector Machine (SVM) achieved the highest overall accuracy, F1-score, and AUC-ROC, indicating superior capability in handling high-dimensional multimodal data. Random Forest closely followed SVM, showing strong robustness and stable performance across cross-validation folds. Logistic Regression produced moderate results, benefiting from its simplicity and interpretability but struggling with complex nonlinear patterns. K-Nearest Neighbours showed the lowest performance, largely due to sensitivity to high dimensionality and feature scaling.

Overall, the results confirmed that combining image-based features with environmental data significantly improved disease prediction accuracy, validating the effectiveness of the multimodal approach.

# Conclusion

This project successfully demonstrated the potential of classical machine learning models for crop disease prediction using multimodal data. By integrating plant leaf image features with environmental variables, the study achieved more accurate and reliable predictions compared to single-modality approaches. Among the evaluated algorithms, Support Vector Machine emerged as the most effective model, followed closely by Random Forest.

The findings highlight that traditional machine learning techniques, when supported by strong feature engineering and proper preprocessing, can serve as computationally efficient, interpretable, and scalable solutions for smart agriculture systems. This work provides a solid foundation for future research, including real-time IoT integration, expanded environmental data, and hybrid deep learning–machine learning frameworks for large-scale agricultural disease monitoring.
