# <div align="center">Credit Card Fraud Detection using Federated Learning</div>

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig4-3.png" alt="Project Logo" width="400"/>
</div>

## <div align="center">Project Overview</div>

This project aims to enhance credit card fraud detection using federated learning, a decentralized approach to machine learning. By leveraging edge computing and advanced algorithms like Federated Averaging (FedAvg) and Synthetic Minority Oversampling Technique (SMOTE), we optimize the detection of fraudulent transactions while maintaining data privacy.

## <div align="center">Implementation Steps</div>

### 1. Banks Grouping

#### 1.1 PSO Algorithm for Bank-Server Assignment

- **Objective**: Assign 600 bank nodes to 90 server nodes, ensuring communication within a 1000-unit range.
- **Visualization**: Final assignments of bank nodes to servers are visualized to verify the algorithm's efficacy.

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig4-1.png" alt="Optimal Assignment of Bank to Server" width="600"/>
</div>

### 2. Implementing SMOTE in Credit Card Fraud Detection

#### 2.1 Preprocessing Steps
- **Data Cleaning**: Handle missing values and outliers.
- **Feature Selection**: Identify relevant features influencing fraud prediction.
- **Normalization**: Scale features to standardize the data.

#### 2.2 Application of SMOTE
- **Parameter Tuning**: Choose the number of nearest neighbours (k) for synthetic sample generation.
- **Synthetic Sample Generation**: Apply SMOTE to the minority class for balanced class distribution.

### 3. Multilayer Perceptron (MLP)

#### 3.1 Model Configuration
- **Input Layer**: Neurons correspond to dataset features.
- **Hidden Layers**: 64 and 32 neurons in the first and second hidden layers, respectively.
- **Output Layer**: Single neuron with a sigmoid activation function for binary classification.
- **Activation Function**: ReLU for hidden layers, sigmoid for the output layer.

#### 3.2 Training Process
- **Optimization Algorithm**: 'adam' optimizer with binary cross-entropy loss.
- **Iterations**: Predefined number of iterations (e.g., 100 for demonstration).

#### 3.3 Model Evaluation
- **Metrics**: Accuracy, precision, recall, and AUC-ROC.

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig4-2.png" alt="MLP Architecture" width="600"/>
</div>

### 4. Federated Averaging

#### 4.1 Aggregation at the Edge Node Level
- **Process**: Aggregate model updates from bank branches, normalize weighted sums, and update local models.

#### 4.2 Aggregation at the Central Server Level
- **Process**: Aggregate updates from edge nodes, normalize weighted sums, and update the global model.

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig4-3.png" width="600"/>
</div>

## <div align="center">Results</div>

### 5.1 Banks Grouping Performance
- **Evaluation**: PSO algorithm evaluated against GA and Jaya Algorithm for cost function minimization and load balance.
- **Visualization**: Graphs comparing the convergence of different algorithms.

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig5-1.png" alt="PSO Performance" width="600"/>
</div>

### 5.2 Performance Evaluation with SMOTE
- **Evaluation**: Comparison of models trained on original vs. SMOTE-enhanced datasets.
- **Visualization**: Performance metrics and ROC curve improvements.

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig5-2.png" alt="SMOTE Performance" width="600"/>
</div>

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig5-2-1.png" alt="SMOTE Performance" width="600"/>
</div>

### 5.3 MLP vs Decision Tree
- **Outcome**: MLP outperforms the decision tree model for fraud detection.
<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig6-1.png" alt="MLP Performance" width="600"/>
</div>
<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig6-2.png" alt="DL Performance" width="600"/>
</div>
### 5.4 Federated Learning Performance
- **Metrics**: Accuracy: 0.8784, Precision: 0.8618, Recall: 0.9010, F1 Score: 0.8810

<div align="center">
  <img src="https://raw.githubusercontent.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning/main/images/Fig7-1.png" alt="FL Performance" width="600"/>
</div>

## <div align="center">Conclusion</div>

Our project demonstrates the potential of federated learning combined with edge computing and advanced machine learning techniques to enhance credit card fraud detection while preserving data privacy. The integration of SMOTE further improves model performance, addressing class imbalance issues. This work lays the foundation for future research in privacy-preserving machine learning methodologies.

## <div align="center">Technologies Used</div>
- **Algorithms**: Federated Averaging (FedAvg), Improved Particle Swarm Optimization (IPSO), SMOTE
- **Machine Learning Models**: Multilayer Perceptron (MLP)
- **Tools**: Python, TensorFlow, scikit-learn
- **Version Control**: GitHub

## <div align="center">Project Repository</div>
- GitHub: [Project Repository](https://github.com/pratapavinesh/Credit-Card-Fraud-Detection-using-Federated-Learning)

## <div align="center">License</div>
Distributed under the MIT License. See `LICENSE` for more information.

---
