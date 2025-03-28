
# Supreme Court Appeals Outcome Prediction

This project builds on a larger initiative (https://github.com/noambassat/VIrtual_Machine_Crawler) where we developed **web crawler**  to scrape all Supreme Court cases in Israel from 1997. The focus here is to predict the outcomes of criminal appeal cases (both direct appeals and requests for appeal) brought before the Supreme Court.

# Supreme Court Classifier

This project includes Jupyter notebooks aimed at developing and evaluating Machine Learning models for classifying Supreme Court decisions. The project involves data exploration, preprocessing, model training, and evaluation.

---

## Project Structure

### Notebooks:
1. **1_explore_and_merge.ipynb**:
   - Initial exploration of the data and merging different datasets to prepare for model training.

2. **2_first_classifier.ipynb**:
   - Development and training of the initial classifier model. This includes feature engineering and selecting the appropriate model.

3. **3_Sample_for_Model_Prediction.ipynb**:
   - Sampling and creating datasets for predictions and model evaluation.

4. **4_explore_and_merge_RAP_AP.ipynb**:
   - Advanced data exploration and merging with a focus on specific subsets.

5. **classifier_model.py**:
   - A Python script containing the implementation of the classifier model.

---

## Key Data Files

- **full_data_with_predictions.xlsx**:
  - A comprehensive dataset including predictions generated by the model.

- **class_distribution_by_year.xlsx**:
  - Analysis of class distribution over different years.

---

## Getting Started


 **Clone the repository**:
   Copy the repository to your local machine using:
   ```bash
   git clone https://github.com/noambassat/SupremeCourtClassifier.git
