# PyCaret-Clustering-Tutorial-Unleashing-the-Power-of-Low-Code-Machine-Learning


PyCaret Clustering Tutorial

PyCaret Logo

Introduction

Welcome to the PyCaret Clustering Tutorial! PyCaret is an open-source, low-code machine learning library in Python designed to streamline and accelerate machine learning workflows. This tutorial focuses on the Clustering Module, an unsupervised machine learning module that excels in grouping similar objects.

Installation

Ensure compatibility with Python 3.7-3.10, Ubuntu 16.04+, or Windows 7+. Install PyCaret using pip, with optional full dependencies for specific use cases:

bash
Copy code
pip install pycaret[full]
Quick Start

PyCaret's Clustering Module offers an intuitive workflow:

Setup: Initialize the training environment and transformation pipeline.
Create Model: Train and evaluate the performance of a chosen model.
Assign Labels: Assign cluster labels to the training data based on the trained model.
Analyze Model: Use various plots to analyze the model's performance.
Prediction: Predict cluster labels on unseen data.
Save Model: Save the entire pipeline for later use.
python
Copy code
from pycaret.clustering import *
s = setup(data, session_id=123)
kmeans = create_model('kmeans')
kmeans_cluster = assign_model(kmeans)
plot_model(kmeans, plot='cluster')
Explore more functionalities, such as the Object-Oriented API, Experiment Logging, Deploying Models, and Saving/Loading Models and Experiments.

Object-Oriented API

PyCaret supports both Functional and Object-Oriented APIs. Experiment seamlessly by importing the ClusteringExperiment class:

python
Copy code
from pycaret.clustering import ClusteringExperiment
exp = ClusteringExperiment()
exp.setup(data, session_id=123)
Experiment Logging

Enable experiment tracking with MLFlow or other loggers by setting log_experiment and experiment_name in the setup:

python
Copy code
s = setup(data, log_experiment='mlflow', experiment_name='clustering_project')
Contribution

Feel free to contribute to this tutorial by raising issues, providing feedback, or submitting pull requests.

License

This tutorial is licensed under the MIT License.

Happy clustering with PyCaret! 🚀
