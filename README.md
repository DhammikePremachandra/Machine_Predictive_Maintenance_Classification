# Machine Predictive Maintenance Classification

## Project Overview
This project aims to classify different types of machine failures using predictive maintenance data. The goal is to identify potential failures before they occur, thereby reducing downtime and maintenance costs. The project utilizes various machine features and implements machine learning models to predict the type of failure.

## Dataset
The dataset contains the following features:
- **Air temperature [K]**
- **Process temperature [K]**
- **Rotational speed [rpm]**
- **Torque [Nm]**
- **Tool wear [min]**
- **Type** (Categorical)
- **Failure Type** (Target variable)

## Project Structure
1. **Importing Libraries**: Import necessary libraries for data manipulation, visualization, and modeling.
2. **Data Loading and Exploration**: Load the dataset and perform initial exploration to understand the data structure and contents.
3. **Data Cleaning**: Handle missing values and ensure data quality.
4. **Data Preprocessing**: Encode categorical variables and normalize numerical features.
5. **Handling Imbalanced Data**: Use SMOTE to handle class imbalance.
6. **Model Training and Hyperparameter Tuning**: Train and tune models using a pipeline and cross-validation.
7. **Model Evaluation**: Evaluate the model using accuracy, classification report, and confusion matrix.
8. **Conclusions**: 
    - The Random Forest classifier achieved an overall accuracy of 96%.

    - Precision, recall, and F1-scores varied across different failure types, with 4 and 5 minority classes being zero accurately predicted. 

    - Majority classes are High accurately predicted.

    - The use of SMOTE helped to mitigate the class imbalance issue.
9. **Challenges and Limitations**:
    - The primary challenge was the imbalanced nature of the target variable, which required careful handling using techniques like SMOTE.

    - Hyperparameter tuning was computationally expensive, requiring strategies to reduce search space and iterations.

10. **Future Improvements**:
    - Collecting more data for minority failure types could help improve model performance.

    - Exploring different algorithms and ensemble methods may yield better results.

    - Further tuning and optimization of hyperparameters can be conducted with more computational resources.

## Getting Started
### Prerequisites
- Python 3.6 or higher
- Jupyter Notebook
- Install the required libraries:
  ```sh
  pip install -r requirements.txt

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/DhammikePremachandra/Machine_Predictive_Maintenance_Classification.git
    cd Machine_Predictive_Maintenance_Classification
2. Install dependencies:
    ```sh
    pip install -r requirements.txt
3. Run the notebook:
    ```sh
    jupyter notebook Machine_Predictive_Maintenance_Classification.ipynb
