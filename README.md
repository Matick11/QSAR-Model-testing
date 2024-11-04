# QSAR-Model-testing
Description
Scripts for evaluating QSAR model performance using different molecular fingerprints. This project provides tools to test the effectiveness of machine learning algorithms on chemical datasets, applying various validation methods and visualizations to compare model performance.

Table of Contents
Introduction
Features
Installation
Usage
Scripts Overview
Parameters and Validation
Results and Visualization
License
Introduction
This project facilitates the testing and evaluation of machine learning models on chemical datasets. By generating molecular fingerprints from SMILES representations, the QSAR (Quantitative Structure-Activity Relationship) models can be trained and assessed to predict properties or activities of chemical compounds. Model performance can be measured and compared across different fingerprints, including MACCS and AtomPair.

Features
Data preparation and cleaning tools for QSAR model training
Conversion of chemical names or CAS numbers into SMILES format
Generation of multiple molecular fingerprints
Testing of model performance with cross-validation and leave-one-out validation
Visualization tools to compare model metrics like R² and RMSE
Installation
Clone this repository:
bash
Copy code
git clone https://github.com/your-username/QSAR-Model-Testing.git
Install required dependencies:
bash
Copy code
pip install -r requirements.txt
Ensure you have necessary chemical informatics libraries (like RDKit) installed.
Usage
Step 1: Data Preparation
Prepare and clean your dataset, saving it as a .csv file. Each chemical compound should be listed with identifiers or CAS numbers.

Step 2: Generate SMILES Representations
To convert chemical names or CAS numbers to SMILES format, use the Converting Name or CAS into SMILES.ipynb notebook. This step is crucial for generating molecular fingerprints.

Step 3: Model Testing
Use one of the following notebooks to test your QSAR models on the prepared datasets:

Avtomatika.ipynb - Comprehensive testing across multiple fingerprints
maccs.ipynb - Testing with MACCS fingerprints
AtomPair.ipynb - Testing with AtomPair fingerprints
Adjust model parameters as needed, and choose between cross-validation and leave-one-out validation methods.

Scripts Overview
Converting Name or CAS into SMILES.ipynb: Converts chemical names or CAS numbers into SMILES for fingerprint generation.
Avtomatika.ipynb: Main script to perform model testing on a prepared dataset.
maccs.ipynb and AtomPair.ipynb: Scripts for testing specific molecular fingerprints.
Plotting.ipynb: Generates heatmaps and radar charts to visualize model performance.
Parameters and Validation
Model Parameters: Modify the model parameters within each notebook to optimize performance.
Validation Methods: Two validation options are available:
Cross-validation: Splits data into multiple training and testing sets.
Leave-one-out: Tests model performance by iterating through individual data points.
Results and Visualization
Compare R² and RMSE metrics from each model and validation method. Use the Plotting.ipynb script to create visualizations:

Heatmaps to show model performance across different parameters and fingerprints
Radar charts to provide an overview of performance metrics
License
This project is licensed under the MIT License - see the LICENSE file for details.
