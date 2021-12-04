# Author Attribution - CMPE 255 Final Project
Team : 

Adarsh Narasimha Murthy [014952275]
Anuhya Gankidi [015897323]
Deepak Vellore Karunamoorthy [014655628]
Sai Harsha Anirudh Garre [015218996]


Authorship attribution is the process of determining the writer of a document. We used The [Reuter C50_50 dataset](https://archive.ics.uci.edu/ml/datasets/Reuter_50_50) for this repository.

# How to Run
- The file Author [Author Attribution.ipynb](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/Author%20Attribution.ipynb) contains the main code.
- The commands to download the auxiliary packages are available in the same notebook.
- Data Preprocessing code is also present in the same file. However since runing it takes considerable amount of time, the code has been run and saved in the CSV files [Preprocessed_trainset.csv](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/preprocessed_trainset.csv) and [Preprocessed_testset.csv](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/preprocessed_trainset.csv). However, if you wish to run it again please uncomment the below lines:
```
  #df_trainset.to_csv('preprocessed_trainset.csv', encoding='utf-8', index=False)
  #df_testset.to_csv('preprocessed_testset.csv', encoding='utf-8', index=False)
 ```
 - The code for generation of LDA training model is available at [LDA.ipyb](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/LDA.ipynb). There was a code conflict to run this locally, hence it was run in google colab and the results stored in [toptopics.csv](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/toptopics.csv)
 

## Approches:
### 1. Feature Engineering - Stylometry +  LDA + Geographic features

![Architecture](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/images/stylometry.jpeg)

#### Results:
![Results](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/images/stylometry_results.PNG)

### 2. Traditional Approach
#### I. Data Preprocessing
  - Special Characters Removal
  - Remove digits and whitespaces
  - Lemmatization

![Data Preprocessing](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/images/data_preproces.jpeg)
#### II. Vectorization
  - Bag of Words
  - TF-IDF
  - Chi-Square

#### III. Dimensionality Reduction
  - SVD
  
 #### IV. Classification Algorithms used and their results:
 
 ![Results](https://github.com/Adarsh3thy/CMPE255-Project/blob/main/images/approach2_results.PNG)
 
  







