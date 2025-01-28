# Predictive Maintenance Project

## Overview
This project explores the implementation of **Predictive Maintenance** strategies to enhance operational efficiency, reduce downtime, and optimize maintenance scheduling in industrial applications. Predictive Maintenance leverages **data-driven techniques** and **machine learning models** to predict equipment failures and recommend preventive actions, ensuring cost-effective and reliable operations.

The dataset is modeled after an existing milling machine with 10,000 data points and 14 features, including parameters like air temperature, process temperature, torque, rotational speed, and tool wear. The goal is to predict **machine failure** based on multiple independent failure modes.


### 1. Data Preparation
- The dataset consists of operational and failure-related features:
  - **Environmental Parameters**: Air and process temperature.
  - **Machine Parameters**: Torque, rotational speed, tool wear.
  - **Failure Labels**: Machine failure (binary label) and subcategories (tool wear failure, heat dissipation failure, etc.).

- Features are normalized and preprocessed using standard techniques to ensure consistent scaling and remove noise.

### 2. Failure Modes
The project models five independent failure modes:
1. **Tool Wear Failure (TWF)**: Based on random wear between 200-240 minutes.
2. **Heat Dissipation Failure (HDF)**: Triggered by specific temperature and rotational speed thresholds.
3. **Power Failure (PWF)**: Occurs when power exceeds operational limits (3500W–9000W).
4. **Overstrain Failure (OSF)**: Triggered by excessive tool wear and torque product.
5. **Random Failure (RNF)**: A small probability-based failure, simulating unexpected breakdowns.

If any of these modes are triggered, the **Machine Failure** label is set to 1.

### Key Features
- Handles **class imbalance** using techniques like **SMOTE (Synthetic Minority Oversampling Technique)** to ensure the minority failure class is well-represented.
- Advanced **failure mode analysis** to understand root causes of machine breakdowns.

### 3. Model Development
The project employs machine learning models, such as:
- **Logistic Regression**: Known for its simplicity and efficiency.
- **Support Vector Machine (SVM)**: Balances precision and recall.
- **Neural Networks (NN)**: Captures complex relationships between features.

### 4. Evaluation Metrics
Models are evaluated using:
- **Accuracy**: Overall correctness of predictions.
- **Precision and Recall**: To minimize false positives and false negatives.
- **F1-Score**: Balance between precision and recall.
- **Matthews Correlation Coefficient (MCC)**: A balanced measure for imbalanced datasets.

## Highlights
### Real-World Applications
- **Manufacturing**: Predict equipment failures to minimize downtime and improve productivity.
- **Energy and Utilities**: Monitor critical machinery to avoid catastrophic failures.
- **Automotive Industry**: Enhance maintenance schedules for better vehicle performance.





1. **Dataset**: The dataset contains 10,000 entries simulating real-world machine operations.
2. **Code and Models**:
   - Preprocessing scripts for data cleaning and feature engineering.
   - Machine learning model implementations with hyperparameter tuning.
3. **Visualization**:
   - Detailed visualizations (e.g., heatmaps, failure distributions) to analyze feature importance and correlations.


## Applications
This project is ideal for industries looking to:
1. Implement **IoT-enabled Predictive Maintenance** systems for real-time monitoring.
2. Optimize spare parts inventory by predicting replacement schedules.
3. Improve product quality and reliability through root cause analysis.
4. Reduce operational costs by minimizing unplanned downtime.


## Contributions
Contributions are welcome! You can:
- Improve the machine learning models.
- Add support for additional failure modes.
- Extend the dataset for other industrial applications.

To contribute, fork the repository, make your changes, and submit a pull request.
