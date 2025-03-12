# Cancer-Diagnosis-project

## Data Description

This project utilizes a dataset to diagnose the cancel type. The dataset comprises **569 instances (rows) with 32 attributes (columns)**, totaling approximately **142.4+ KB** in size.

The dataset is structured as follows:

* **31 Feature Columns:** These columns represent quantitative features extracted from the digitized images of the FNA samples. Each feature describes characteristics of the cell nuclei present in the image, such as:
    * Radius
    * Texture
    * Perimeter
    * Area
    * Smoothness
    * Compactness
    * Concavity
    * Concave points
    * Symmetry
    * Fractal dimension
    * And their respective standard error and worst values.
* **Target Vector (Diagnosis):** This column represents the diagnostic outcome, categorizing the breast mass as either:
    * **Benign (B):** Indicating a non-cancerous mass.
    * **Malignant (M):** Indicating a cancerous mass.

## Data Exploration and preprocessing:
* As the data features are numerical values, So I used the **correlation coefficient** to perform **feature selection** to reduce the feature matrix.
* Encode the **Diagnosis** coulumn to 1 for M and 0 for B, to be used in the ML.
* Creating a new dataframe with **only 7 features**, with the heighest values of correlation with the Diagnosis, and the encoded target vector.
* Data size after all preprocessing is **35.7 KB**. 


## Machine Leaning:

*  I developed 4 ML models
  
**Naive Bayes**: Acc= 0.94

**Decision Tree**: Acc= 0.909 and after hyperparameter Acc= 0.93

**Random Forest**: Acc= 0.93

**Logistic Regression**: Acc= 0.93

* Evaluate the confusion Matrix for each.  






































