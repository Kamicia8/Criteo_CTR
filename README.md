# Criteo_CTR

This project was developed by **Izabela Wyderka**, **Kamila Ćwikła** and **Klaudia Stodółkiewicz** as part of the **Data Exploration** course during the first semester of the Master's studies in **Data Science** at **AGH University of Technology in Kraków**.

It focuses on analyzing data related to CTR (Click-Through Rate) in display advertising. The goal is to explore various methods for handling high-cardinality data, such as hashing techniques. Additionally, logistic regression with regularization will be used to improve model generalization and prevent overfitting. Different optimization approaches, including the F1 score, will be examined to assess model performance.

For this project, we performed our analysis on a sample of approximately 2 million rows taken from the original 45-million-row training dataset (file: `main_dataset_2M_analysis.ipynb`).

Additionally, since the Criteo CTR dataset is already fully encoded, we decided—purely for learning purposes—to analyze a small unencoded dataset, which we manually explored and encoded (file: `side_data_analysis.ipynb`).

Files such as `pca.ipynb`, `smote_lasso.ipynb` and `data_cleaning.ipynb` contain separate analyses of specific tools and techniques. These were used to identify the most effective parameters and methods to apply in the final modeling process.

## Instructions for Downloading the Dataset

### Step 1: Install Kaggle API

Make sure you have the Kaggle API installed. If you haven't installed it yet, you can do so via pip:

```
pip install Kaggle
```

### Step 2: Set Up Kaggle API Key

1. Go to your [Kaggle account settings](https://www.kaggle.com/settings).

2. Scroll down to the "API" section and click on Create New API Token.

3. This will download a `kaggle.json` file containing your API credentials.

4. Place this `kaggle.json` file in the `~/.kaggle/` directory. If the directory does not exist, create it.

### Step 3: Download the Dataset

Once your API key is set up, you can download the dataset using the following command:
```
kaggle datasets download -d mrkmakr/criteo-dataset
```
This command will download the dataset as a ZIP file. Unzip the file to access the data.

## Command to run Docker container

```
docker run -p 8888:8888 -p 4040:4040 -v ${PWD}:/home/jovyan/work jupyter/all-aprk-notebook
```





