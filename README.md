# Machine Learning Prediction Model on Human Activity Recognition using Wearable Sensor Technology Data

This project aims to build a prediction model using wearable sensor technology data to recognize human activities. 

Two tasks are to be completed using the provided dataset:

1. **Binary Classification**: Classify the activity of each time window into static (0) and dynamic (1). For this task, postural transitions are considered as static (0).
2. **Multi-class Classification**: Classify walking (1), walking_upstairs (2), walking_downstairs (3), sitting (4), standing (5), lying (6), and static postural transition (7).

# Getting Started

## Dataset

The dataset consists of the following files:

- **'training_data.txt'**: Training dataset

* **'test_data.txt'**: Data set to be predicted

+ **'data_dictionary.txt'**: Introduction of the dataset

- **'features_info.txt'**: Detailed information about each variable

## Running the Code

To run the Rmd files, download the following files:

- **'test_data.txt'**

* **'training_data.txt'**

+ **'Binary.Rmd'**

- **'multi_class.Rmd'**

Ensure that the Rmd file and the txt data file are in the same path. Running each Rmd file will generate a txt file, which is the prediction result of the prediction data for different tasks.

## Notice

***'Binary.Rmd' will take 30 mins when running.***

***'multi_class.Rmd' will take 1--2 hours when running.***

Running **'Binary.Rmd'** will get **"binary.txt"**

Running **'multi_class.Rmd'** will get **"multiclass.txt"** file.

***When running **'multi_class.Rmd'**, you need to run **'Binary.Rmd'** first since you need to load **"binary.txt"** in **'multi_class.Rmd'**.***

## Prerequisites

**Rstudio**

## Installing

Install and run the following packages in **RStudio** to support running **'binary.Rmd'** and **'multi_class.Rmd'** files:

```{r}
install.packages('caret')
install.packages('caretEnsemble')
install.packages('glmnet')
install.packages('readr')
```

# Method

- For task 1, construct the **C5.0 algorithm** to complete the binary classifier task.

* For task 2, build **generalized linear models** to complete the multi-class classifier task.

# Performance

Through continuous optimization, 100% accuracy in task 1 and 95.7% in task 2 were obtained on the Leaderboard.

- **'binary.txt'** is the predict result for Task 1.

* **'multiclass.txt'** is the predict result for Task 2.