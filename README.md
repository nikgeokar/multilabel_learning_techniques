# Multilabel Learning Techniques

### Objective

This notebook focused on multilabel classification using the DeliciousMil dataset. The primary objective is to compare the performance of various machine learning models when combined with the ChainClassifier approach.

### Dataset Overview

The DeliciousMil dataset serves as the foundation for our analysis. It comprises a collection of documents, each associated with multiple labels. The dataset is widely used in the field of text classification and provides an excellent opportunity to evaluate the performance of different models.

### Feature Extraction

To facilitate the multilabel classification task, we employ the TF-IDF (Term Frequency-Inverse Document Frequency) technique to transform the documents into numerical feature vectors. The TF-IDF approach calculates the importance of each word in a document by considering both its frequency within the document and its rarity across the entire dataset. This transformation enables us to represent the textual data in a format suitable for training machine learning models.

### Models and Approaches

In this notebook, we focus on the ChainClassifier approach combined with various machine learning models for multilabel classification. The ChainClassifier considers the label order and dependencies when making predictions. It trains a sequence of binary classifiers, where the prediction of each classifier is conditioned on the predictions of the previous classifiers. This approach captures the label correlations present in the data.

We compare the performance of the ChainClassifier combined with the following machine learning models:

<li>LogisticRegression</li>
<li>DecisionTreeClassifier</li>
<li>RandomForestClassifier</li>
<li>KNeighborsClassifier</li>
