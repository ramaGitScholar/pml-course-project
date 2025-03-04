# **pml-course-project**  
A project based on *Practical Machine Learning (Johns Hopkins University)* course from Coursera.

## **Machine Learning Project - Weight Lifting Exercise Classification**

### **Project Overview**  
This project aims to predict the manner in which individuals performed weightlifting exercises based on sensor data from accelerometers placed on different parts of the body. The dataset is derived from the *Weight Lifting Exercise Dataset*.

---

## **Dataset**
- **Training Data**: [Download Here](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv)  
- **Test Data**: [Download Here](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv)  
- **Source**: [Groupware@PUC-Rio](http://groupware.les.inf.puc-rio.br/har)  

---

## **Project Components**
1. **Data Preprocessing**
   - Removing metadata and columns with excessive missing values  
   - Handling near-zero variance predictors  
   - Splitting data into training and testing sets  
   - Imputing missing values  

2. **Model Training**
   - Random Forest (`rf`)  
   - Gradient Boosting Machine (`gbm`)  
   - Cross-validation for performance tuning  

3. **Evaluation & Prediction**
   - Model accuracy assessment using confusion matrices  
   - Applying the trained model to predict test data  
   - Generating submission file for the *Course Project Prediction Quiz*  

---

## **Reproducibility**
- The analysis and results are documented in an **R Markdown** file:  
  **`coursera_pml_project.rmd`**  
- The compiled **HTML** report:  
  **`coursera_pml_project.html`**  
  contains all details of the model-building process.

---

## **Submission Instructions**
1. Upload **`coursera_pml_project.rmd`** and **`coursera_pml_project.html`** to GitHub.  
2. Ensure that the `gh-pages` branch is enabled for easy access to the HTML file.  
3. Submit the GitHub repository link for grading.  

---

## **Dependencies**
Ensure the following R packages are installed before running the analysis:  
```r
install.packages(c("caret", "randomForest", "gbm", "dplyr", "ggplot2", "rmarkdown"))
```

---

## **Running the Analysis**
To generate the HTML report, execute the following command in R:  
```r
rmarkdown::render("coursera_pml_project.rmd")
```

---

## **Final Predictions**
- The predictions for the test set are saved in:  
  **`final_predictions.csv`**  

---

## **License**
This project follows the dataset usage guidelines from [Groupware@PUC-Rio](http://groupware.les.inf.puc-rio.br/har).  

---
