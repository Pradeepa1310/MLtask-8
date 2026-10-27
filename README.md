# Phishing Website Detection Using Machine Learning

## Project Overview
This project uses Machine Learning to detect phishing websites and distinguish them from legitimate websites. A Linear Support Vector Machine (Linear SVM) classifier is trained using numerical features from the PhiUSIIL Phishing URL Dataset.

## Objectives
- Detect phishing websites using machine learning.
- Preprocess the dataset and handle missing values.
- Train and test a Linear SVM classification model.
- Evaluate model performance using classification metrics.
- Visualize the confusion matrix and ROC curve.

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

## Dataset
**Dataset:** PhiUSIIL Phishing URL Dataset

The dataset contains website-related information used to classify websites as legitimate or phishing.

The project removes non-numeric columns such as URL, Domain, TLD, and Title from the model features. Missing values in the target column are removed, and missing numerical feature values are filled using their median.

**Note:** Download the dataset separately and upload it to your working environment before running the notebook.

## Project Workflow
1. Import the required Python libraries.
2. Load and explore the dataset.
3. Check missing values and class distribution.
4. Separate the target variable and numerical features.
5. Handle missing and infinite values.
6. Split the data into training and testing sets.
7. Standardize features using `StandardScaler`.
8. Train a Linear SVM model using `LinearSVC`.
9. Predict website classifications.
10. Evaluate the model and visualize the results.

## Machine Learning Algorithm
**Linear Support Vector Machine (Linear SVM)**

The model uses `LinearSVC` with balanced class weights to help address class imbalance. A pipeline combines feature standardization and model training.

## Evaluation Metrics
The model is evaluated using:

- **Precision:** Measures how many predicted phishing cases are correct.
- **Recall:** Measures how many actual phishing cases are detected.
- **F1 Score:** Combines precision and recall.
- **ROC-AUC:** Measures the model's ability to distinguish between the two classes.
- **Confusion Matrix:** Shows correct and incorrect classifications.
- **Classification Report:** Provides precision, recall, and F1 score for each class.

The notebook also displays an ROC curve to visualize classification performance.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn
   ```

3. Download the PhiUSIIL Phishing URL Dataset.
4. Update the dataset file path in the notebook to match your local environment.
5. Open `Task8_ML.ipynb` using Jupyter Notebook or Google Colab.
6. Run all cells in order to train and evaluate the model.

## Results
The notebook generates a confusion matrix, classification report, precision, recall, F1 score, ROC-AUC score, and ROC curve.

The actual numerical performance results should be added here after running the notebook.

## Conclusion
This project demonstrates how machine learning can be applied to phishing website detection using numerical website features. The Linear SVM model is trained and evaluated to identify phishing websites and distinguish them from legitimate websites.

## Future Improvements
- Compare Linear SVM with other classification algorithms.
- Perform feature selection and hyperparameter tuning.
- Evaluate the model on additional datasets.
- Develop a simple web application for phishing URL detection.

## Author
Pradeepa D
