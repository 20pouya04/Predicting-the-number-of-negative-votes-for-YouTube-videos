# YouTube Video Dislike Prediction  

## Overview  
This project aims to build a machine learning model to predict the number of dislikes on YouTube videos based on various features such as uploader statistics, view counts, and video metadata. The main goal is to assist content creators and marketers in understanding viewer engagement and improving video performance.  

## Dataset  
The dataset consists of two CSV files: `train.csv` and `test.csv`. The training set is used to build and evaluate the model, while the test set helps to validate predictions. The dataset contains various features related to video performance and viewer interaction.  

### Key Features:  
- **video_id**: Unique identifier for each video.  
- **uploader_sub_count**: Number of subscribers the uploader has.  
- **view_count**: Total number of views the video has received.  
- **like_count**: Total number of likes the video has received.  
- **dislike_count**: Total number of dislikes the video has received (target variable).  
- **upload_date**: Date the video was uploaded.  
- **category**: Category under which the video is classified (e.g., Music, Education, Entertainment).  
- **duration**: Length of the video in seconds.  
- **tags**: Keywords associated with the video.  

## Project Workflow  
1. **Data Preprocessing**  
   - Loaded and inspected the data.  
   - Handled missing values and performed data normalization.  
   - Removed outliers using Isolation Forest and Local Outlier Factor methods.  

2. **Feature Engineering**  
   - Mapped boolean features to binary values and dropped unnecessary columns.  
   - Created new features to enhance model performance.  

3. **Modeling**  
   - Implemented various regression techniques:  
     - Linear Regression  
     - Polynomial Regression  
     - Ridge Regression  
     - Lasso Regression  
     - ElasticNet Regression  

4. **Model Evaluation**  
   - Evaluated models using metrics such as Mean Absolute Error (MAE), Maximum Error, and R² Score.  
   - Visualized predictions against actual dislike counts to assess model performance.  

## Results  
Provided a comprehensive comparison of various regression models and their performance metrics. Identified the most effective models for predicting dislike counts on YouTube videos.  

## Future Work  
- **Hyperparameter Tuning**: Further improve model performance through fine-tuning.  
- **Feature Engineering**: Explore additional features that could enhance prediction accuracy.  
- **Model Interpretation**: Use SHAP values to interpret model predictions and understand feature importance.  

## How to Use  

### Prerequisites  
- Python 3.6+  
- Required libraries: numpy, pandas, seaborn, matplotlib, scikit-learn  

### Installation  
Clone the repository and install the required libraries:  
```bash  
git clone https://github.com/20pouya04/Predicting-the-number-of-negative-votes-for-YouTube-videos.git   
cd Predicting-the-number-of-negative-votes-for-YouTube-videos   
pip install -r requirements.txt
