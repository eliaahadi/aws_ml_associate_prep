# AWS ML Associate --- Section 2.1: Choose a Modeling Approach

This section covers how to choose the right machine learning modeling
approach based on the problem type, data characteristics, and business
objectives. It focuses on classification, regression, clustering, and
recommendation systems, and aligns them with AWS services and
algorithms.

## Problem Types & Approaches

• Classification --- predict categories (e.g., fraud detection,
sentiment analysis)

\- Algorithms: Logistic Regression, XGBoost, Linear Learner
(classification), Deep Learning (CNN/RNN for text/images)

• Regression --- predict continuous values (e.g., price forecasting,
demand prediction)

\- Algorithms: Linear Regression, XGBoost (regression), Deep Learning
(dense networks)

• Clustering --- group unlabeled data (e.g., customer segmentation)

\- Algorithms: K-Means, PCA for dimensionality reduction

• Recommendation Systems --- personalized ranking (e.g., product
recommendations)

\- Algorithms: Factorization Machines, Neural Collaborative Filtering

## Factors in Choosing an Approach

• Type of output variable (categorical vs continuous vs none)

• Availability of labeled data (supervised vs unsupervised)

• Scale of data (large-scale may require distributed deep learning)

• Interpretability requirements (linear/logistic vs deep learning
black-box models)

• Latency/performance needs (real-time inference may favor lighter
models)

## AWS Services & Tools

• SageMaker Autopilot --- automatically chooses best model and approach
for tabular data

• SageMaker JumpStart --- pre-trained models for common tasks (vision,
NLP, etc.)

• Built-in Algorithms --- XGBoost, K-Means, Factorization Machines,
Linear Learner

• Framework Containers --- TensorFlow, PyTorch, MXNet, Scikit-Learn

## Exam Tips

• Classification = categorical outputs; Regression = continuous outputs;
Clustering = unsupervised grouping

• Factorization Machines are key for sparse data/recommendation problems

• Use K-Means for clustering; PCA for dimensionality reduction

• Autopilot can simplify model selection for structured tabular problems

• Always align approach with business problem and evaluation metric
(accuracy, RMSE, etc.)
