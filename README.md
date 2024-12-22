
# Supreme Court Appeals Outcome Prediction

This project builds on a larger initiative (https://github.com/noambassat/VIrtual_Machine_Crawler) where we developed **web crawler**  to scrape all Supreme Court cases in Israel from 1997. The focus here is to predict the outcomes of criminal appeal cases (both direct appeals and requests for appeal) brought before the Supreme Court.

Supreme Court Classifier
This repository contains a series of Jupyter notebooks dedicated to developing and evaluating machine learning models aimed at classifying decisions of the Supreme Court. The project encompasses data exploration, preprocessing, model training, and evaluation.

Repository Structure
1_explore_and_merge.ipynb: Initial data exploration and merging of datasets to prepare for model training.

2_first_classifier.ipynb: Development and training of the initial classification model, including feature engineering and model selection.

3_Sample_for_Model_Prediction.ipynb: Sampling strategies implemented to create datasets for model prediction and validation.

4_explore_and_merge_RAP_AP.ipynb: Advanced data exploration and merging, focusing on specific subsets of the data.

classifier_model.py: Python script containing the implementation of the classifier model.

Data Files
full_data_with_predictions.xlsx: Comprehensive dataset including model predictions.

class_distribution_by_year.xlsx: Analysis of class distribution over different years.

Getting Started
To explore the notebooks and replicate the analyses:

Clone the repository:

bash
Copy code
git clone https://github.com/noambassat/SupremeCourtClassifier.git
Navigate to the project directory:

bash
Copy code
cd SupremeCourtClassifier
Install the required dependencies: Ensure you have a Python environment set up with the necessary packages. You can use pip to install the required packages:

bash
Copy code
pip install -r requirements.txt
Note: If a requirements.txt file is not provided, you may need to manually install packages as you encounter import errors when running the notebooks.

Open the notebooks: Launch Jupyter Notebook or JupyterLab:

bash
Copy code
jupyter notebook
or

bash
Copy code
jupyter lab
Then, open the desired notebook to explore the analyses.

Contributing
Contributions to enhance the project are welcome. Feel free to fork the repository, make improvements, and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Note: This README provides an overview of the project structure and instructions to get started. For detailed explanations and results, please refer to the individual notebooks.
