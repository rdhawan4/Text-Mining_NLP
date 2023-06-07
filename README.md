# Text Mining using Natural Language Processing
Natural Language Processing : Incorporating textual semi-structured data into classification model using Natural Language Toolkit library (NLTK)
<br>

<img src="https://user-images.githubusercontent.com/112804900/203012392-3c10dd2c-d9a7-4696-a9a7-1f2f2e8aac81.png" width=600)>

## Implementation
Our goal is to accurately determine whether the customer cancels the subscription or not. 
- We will extract useful information from the "comments.csv" text data which contains information about the recent interaction of the customer with customer service team. We need to transform the semi-structured data into a usable matrix in order to incorporate with the customers personal data.
- Secondly, we have to preprocess the Customer data which may contain categoriacl data points as well.
- Combine transformed text data and numerical personal data by matching the Customer ID on both datatsets.
- Feature Selection using **Filter** and **Wrapper** methods
- Model Development & Evaluation : **Decision Tree, Random Forest & Gradient Boosting**

<img src="https://user-images.githubusercontent.com/112804900/203015469-29d9e406-4c3c-4b1c-bf7c-93a1a5e3301b.png" width=900>

## Improvement in Classification with text data

<img src="https://user-images.githubusercontent.com/112804900/202992612-5e8fd4e4-0e6c-4a99-8d38-5eb0b0f39c7e.png" width=500 >

### Model Performance

| Model Name | Feature Selection Method |No. of k Features| Accuracy Score |
| :---: | :---: | :---: |:---: |
| RandomForestClassifier | None |None | 0.87 |
| GradientBoostingClassifier |  None |None | 0.87 |
| DecisionTreeClassifier |  None |None | 0.87 |
| | | | |
| RandomForestClassifier |  Kbest | 25| 0.80 |
| GradientBoostingClassifier | Kbest | 25 | 0.82|
| DecisionTreeClassifier |Kbest | 25 | 0.82|
| RandomForestClassifier |Kbest | 50 | 0.86|
| GradientBoostingClassifier |Kbest | 50 | 0.87|
| DecisionTreeClassifier |Kbest | 50 | 0.87|
| | | | |
| RandomForestClassifier |SelectFromModel | 10 | 0.88|
| GradientBoostingClassifier |SelectFromModel | 10 | 0.88|
| DecisionTreeClassifier |SelectFromModel | 10 | 0.84|
| RandomForestClassifier |SelectFromModel | 25 | 0.92|
| GradientBoostingClassifier |SelectFromModel | 25 | 0.89|
| DecisionTreeClassifier |SelectFromModel | 25 | 0.88|

## Note <br>
Main Testcode : TextMining.ipynb <br>
Datasets available in Data folder <br>

