# Human-Fall-Detection-and-Classification-based-on-Daily-Activities-using-AWS-Cloud
**Problem**:
Falls can happen in different scenarios, such as walking, standing, or other common
daily activities. The challenge lies in distinguishing a genuine fall event from regular activities
involving similar motions but not falls. The main problem addressed in this project
is the accurate detection of human falls from daily activities. The system needs to be reliable,
real-time capable, and applicable to various environments, ensuring the safety and well-being of
vulnerable individuals.

**Solution**:
This project aims to develop a robust fall detection system based on a pre-existing dataset of
human daily activities that includes fall instances. The goal is to build a machine learning model
that can accurately classify fall events from non-fall activities using the available dataset. By
leveraging the dataset, we can focus on data preprocessing, feature engineering, and model
development, leading to an efficient and cost-effective fall detection solution.


**Methodology**:
The proposed solution involves the development of a fall detection and classification system that
utilizes sensor data from wearable devices such as accelerometers, gyroscopes, and possibly
other biometric sensors. The system will consist of the following components:
Data Preprocessing in the Cloud: Leverage cloud computing resources to preprocess the existing
dataset efficiently. This may include data cleaning, handling missing values, and data
augmentation techniques to improve the dataset's quality and diversity.
Feature Engineering on the Cloud: Perform feature engineering on the cloud platform to extract
relevant features from the preprocessed dataset. Cloud resources can accelerate feature extraction
processes, especially for large datasets.
Cloud-based Machine Learning Models: Implement and train various machine learning
algorithms on the cloud using the extracted features and labelled data. The cloud-based training
process can take advantage of distributed computing to speed up model training. We plan on
implementing k-nearest neighbours (k-NN), logistic regression, quadratic discriminant analysis
(QDA), linear discriminant analysis (LDA), support vector classifier (SVC), and random forest
machine learning techniques to detect falls as well as categorize activities of daily living (ADLs).


**Dataset**:
https://www.kaggle.com/datasets/saadmansakib/smartphone-human-fall-dataset
The original dataset contained around 190 instances of each of these activities performed by 11
individuals. Each instance in the dataset is a 6-second window containing tri-axial accelerometer
and gyroscope data (keeping maximum acceleration magnitude and gyroscope magnitude at the
4th second). The informative features from each of these data windows are:
1. acc_max: Maximum acceleration magnitude of 4th second of the window.
2. acc_kurtosis: Acceleration kurtosis of the whole window.
3. acc_skewness: Acceleration skewness of the whole window.
4. gyro_max: Maximum gyroscope magnitude of 4th second of the window.
5. gyro_kurtosis: Gyroscope kurtosis of the whole window.
6. gyro_skewness: Gyroscope skewness of the whole window.
7. lin_max: Maximum linear acceleration (acceleration excluding gravity) of 4th second of
the window.
8. post_lin_max: Maximum linear acceleration of the 6th second.
9. post_gyro_max: Maximum gyroscope magnitude of the 6th second.
10. fall: 1 if the activity is a fall activity; otherwise, 0.
11. label: The activity label
