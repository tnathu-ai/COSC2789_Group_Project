# Assignment 3: Group Project - COSC2789

# Machine Learning Pipeline - Data Analysis

In the following notebooks, we will go through the implementation of each of the steps in the Machine Learning Pipeline. 

We will discuss:

1. **Data Analysis**
2. Feature Engineering
3. Feature Selection
4. Model Training
5. Obtaining Predictions / Scoring

# Data
+ We will use the house price dataset available on [Kaggle.com](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data). See below for more details.

+ The data from that dataset comes from real estate listings posted on [Alo Nhà Đất](https://alonhadat.com.vn) that was crawled in August 2020 by [Le Anh Duc](https://www.kaggle.com/ladcva)

===========================================================================

## Predicting Sale Price of Houses

The aim of the project is to build a machine learning model to predict the sale price of homes based on different explanatory variables describing aspects of residential houses.


### Why is this important? 

Predicting house prices is useful to identify fruitful investments or to determine whether the price advertised for a house is over or under-estimated in Hanoi.


### What is the objective of the machine learning model?

We aim to minimise the difference between the real price and the price estimated by our model. We will evaluate model performance with the:

### Metrics
Metrics like accuracy, precision, recall are good ways to evaluate classification models for balanced datasets, but if the data is imbalanced and there’s a class disparity, then other methods like ROC/AUC, Gini coefficient perform better in evaluating the model performance.


### How do I download the dataset?

**Instructions also in the lecture "Download Dataset" in section 1 of the course**

- Visit the [Kaggle Website](https://www.kaggle.com/ladcva/vietnam-housing-dataset-hanoi).

- Remember to **log in**.

- The download the file called **'VN_housing_dataset.csv'** and save it in the directory with the notebooks.



**Note the following:**

-  You need to be logged in to Kaggle in order to download the datasets.
-  You need to accept the terms and conditions of the competition to download the dataset
-  If you save the file to the directory with the jupyter notebook, then you can run the code as it is written here.






# Target variable
`Price_range`

# Problem Type
Classification 



# Key Findings:




# Application



## Future improvement:
+ I would like to try out more stacking and ensemble methods to improve the model.

## Productionization

In this step, I built a flask API endpoint that was hosted on a local webserver 

# WORKING ON YOUR LOCAL COMPUTER

python version 3.8.8

1. Install Conda
   by [following these instructions](https://conda.io/projects/conda/en/latest/user-guide/install/index.html). Add Conda
   binaries to your system `PATH`, so you can use the `conda` command on your terminal.

2. Install jupyter lab and jupyter notebook on your terminal

+ `pip install jupyterlab`
+ `pip install jupyter notebook`

### Jupyter Lab

1. Download the 3879312 zipped project folder. Unzip it by double-clicking on it.

2. In the terminal, navigate to the directory containing the project and install these packages and libraries

```
pip install -r requirements.txt
```

3. Enter the newly created directory using `cd directory-name` and start the Jupyter Lab.

```
jupyter lab

```

You can now access Jupyter's web interface by clicking the link that shows up on the terminal or by
visiting http://localhost:8888 on your browser.

4. Click on assignment2.ipynb in the browser tab. This will open up my main file in the Jupyter Lab.

### Note: If the Jupyter Notebook is not responding due to many requests

Error [(The page is not responding)](https://stackoverflow.com/questions/48615535/jupyter-notebook-takes-forever-to-open-and-then-pages-unresponsive-mathjax-i)

I had to restart the notebook; and it did not work. This is because I was printing out too much and the following
scripts resolved the issue by clear out all the output to run through the whole kernal:

1. `conda install -c conda-forge nbstripout` or `pip install nbstripout`

2. `nbstripout filename.ipynb`



## Repository Structure
```
├── dash
│   ├── app.py
│   ├── .gitignore
│   ├── Procfile
│   └── requirements.txt
├── data
│   ├── 
│   └── requirements.txt
├── images
├── README.md
├── interactive_html
│   ├── 
└── cleaning.ipynb
└── encoding.ipynb
└── EDA.ipynb
└── dash_visualization.ipynb
└── function.py
```

