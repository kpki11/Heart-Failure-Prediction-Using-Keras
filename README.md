# Heart-Failure-Prediction-Using-Keras

**Project Overview:**
In this project, I developed machine learning models to predict heart conditions using a synthetic Heart Failure Prediction Dataset sourced from the Antigranular site. The dataset includes anonymized health indicators such as age, sex, blood pressure, cholesterol levels, blood sugar, and peak heart rate. The primary aim was to build accurate predictive models for heart disease while ensuring data privacy through the use of synthetic data.

**Objectives:**
- Develop robust models that accurately predict the likelihood of heart disease based on the provided health indicators.
- Maintain data privacy by exclusively using synthetic data, which simulates real-world health data without exposing actual personal information.

**Dataset Details:**
The Heart Failure Prediction Dataset comprises the following features:
- **Age (N):** Numerical representation of the individual's age.
- **Sex (0/1):** Gender indicator (0 for female, 1 for male).
- **Blood Pressure (mm/Hg):** Recorded blood pressure in millimeters of mercury.
- **Cholesterol (mg/dl):** Cholesterol levels measured in milligrams per deciliter.
- **Blood Sugar (mg/dl):** Blood sugar levels in milligrams per deciliter.
- **Peak Heart Rate (Beats per minute):** Maximum heart rate achieved by the individual.
- **Heart Condition (0/1):** Binary label indicating the presence of heart disease (0 for no heart disease, 1 for heart disease).

This synthetic dataset serves as a valuable tool for healthcare professionals to identify patients at risk and supports researchers in exploring the relationships between various medical and demographic factors and the likelihood of developing heart disease.

**Approach and Implementation:**

- **Data Exploration and Preparation:**
  - **Exploration:** I conducted an initial exploration of the dataset to understand the distribution and correlation of features. This included analyzing statistical summaries and visualizing data distributions to gain insights into the dataset's structure.
  - **Preprocessing:** The data was preprocessed by normalizing features to ensure that all input variables are on a similar scale. I also split the dataset into training and test sets to evaluate the model's performance accurately. This involved standard techniques like stratified sampling to maintain class distribution across both sets.

- **Model Development:**
  - **Convolutional Neural Network (CNN):** While CNNs are typically used for image data, their capability to capture hierarchical features made them suitable for this task. The CNN was designed as follows:
    - **Feature Extraction:** Convolutional layers were used to extract meaningful features from the input data. Filters applied during these layers help detect patterns in the data, such as relationships between age, blood pressure, and other health indicators.
    - **Pooling Layers:** Pooling layers followed the convolutional layers to reduce the dimensionality of the feature maps. This operation summarized the feature maps, reducing computational load and highlighting the most critical information.
    - **Fully Connected Layers:** After feature extraction and pooling, fully connected layers combined the extracted features to perform the final classification. These layers used learned weights to make predictions about heart disease presence.

- **Binary Classification:**
  - **Processing Attributes:** The CNN model was trained to classify input features into two categories: "heart disease" and "no heart disease." During training, the model adjusted its weights based on errors in predictions to learn distinguishing patterns between the two classes. This process involved optimizing the model's parameters to minimize classification errors.

- **Accuracy Achievement:**
  - **Performance:** The CNN model achieved an accuracy of over 90%. This high accuracy demonstrates the model's effectiveness in learning complex patterns and making reliable predictions about heart conditions based on the synthetic dataset. The performance metrics validated the model's ability to generalize well to unseen data.

**Outcome:**
This project highlighted my skills in developing and implementing machine learning models for predictive analytics. The use of a CNN to handle non-image data demonstrated the versatility of deep learning techniques in various domains. The successful implementation and high accuracy of the model underscore its potential for real-world applications, such as predicting heart disease and assisting healthcare professionals in risk assessment. The project also exemplified my commitment to data privacy, given the use of synthetic data sourced from the Antigranular site.
