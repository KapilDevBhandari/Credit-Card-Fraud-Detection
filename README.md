## Credit-Card-Fraud-Detection

This project develops a machine learning model to detect fraudulent credit card transactions using Logistic Regression. It specifically tackles the challenge of highly imbalanced data through undersampling and evaluates model performance using metrics crucial for fraud detection.

📌 Project Purpose
The primary goals of this project are:

Real-time Fraud Detection: To build a robust system capable of identifying fraudulent credit card transactions as they occur.
Handling Imbalanced Data: To effectively address the common problem of highly skewed datasets in fraud detection (where legitimate transactions vastly outnumber fraudulent ones, typically ~99.8% vs. ~0.2%).
Demonstrating Preprocessing: To showcase essential data preprocessing techniques, including feature scaling and undersampling, which are vital for improving model accuracy and reliability on imbalanced datasets.
Appropriate Evaluation: To utilize and emphasize evaluation metrics like Precision, Recall, and F1-score, which provide a more accurate assessment of model performance on the minority (fraudulent) class compared to simple accuracy.

💾 Dataset
This project typically uses a publicly available dataset of credit card transactions (often sourced from European cardholders in September 2013). The dataset contains anonymized transaction features (V1-V28, resulting from a PCA transformation), along with Time (seconds elapsed between each transaction and the first transaction in the dataset) and Amount (the transaction amount). The crucial Class column indicates whether a transaction is fraudulent (1) or legitimate (0).

And you can access the dataset by this link (https://drive.google.com/file/d/10B6teubfXnp3F7wfgL4jajqQMOKdXxw2/view?usp=drive_link)
Or this data is taken from kaggle by searching credit card fraud data.

🛠️ Dependencies

Ensure you have Python 3.x installed. You can install the necessary libraries using pip:
pip install numpy pandas scikit-learn
and if you have already then import it.

🚀 How to Run
Follow these steps to set up and run the project locally:

Clone the Repository:git clone https://github.com/KapilDevBhandari/Credit-Card-Fraud-Detection.git
cd credit-card-fraud-detection

Install Dependencies:
install or import all the dependencies as necessary or you can look in the aviable code file to look for the dependencies.

Execute the Project:
Open the primary Jupyter Notebook (e.g., fraud_detection_notebook.ipynb) to explore the data, run the preprocessing steps, train the model, and evaluate its performance.

📊 Results and Evaluation
Given the severe class imbalance, simple accuracy can be misleading. Therefore, the model's performance is primarily evaluated using metrics that specifically assess its ability to detect the minority (fraudulent) class:

* Precision: Measures the proportion of correctly identified fraudulent transactions among all transactions predicted as fraudulent. A high precision minimizes false positives (legitimate transactions incorrectly flagged as fraud).

* Recall (Sensitivity): Measures the proportion of actual fraudulent transactions that were correctly identified. High recall ensures that most fraudulent activities are caught.
  
* F1-Score: The harmonic mean of Precision and Recall, providing a balanced measure that considers both false positives and false negatives.
  
* Confusion Matrix: A visual representation that helps understand the counts of True Positives (correctly identified fraud), True Negatives (correctly identified legitimate), False Positives (legitimate transactions identified as fraud), and False Negatives (fraudulent transactions missed).

By focusing on these metrics, we aim to achieve a model that effectively minimizes financial losses due to fraud while keeping false alarms at an acceptable level.
