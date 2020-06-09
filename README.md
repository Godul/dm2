# Abstracts Labeling - Data Mining 2019/2020 Project

## Project description

Data for this project consists of two tables in a tab-separated columns format. Each row in those files corresponds to an abstract of a scientific article from ACM Digital Library, which was assigned to one or more topics from the ACM Computing Classification System.

The training data (`DM2020_training_docs_and_labels.csv`) has three columns: the first one is an identifier of a document, the second one stores the text of the abstract, and the third one contains a list of comma-separated topic labels.

The test data (`DM2020_test_docs.csv`) has a similar format, but the labels in the third column are missing.

The task and the format of submissions: the task for you is to predict the labels of documents from the test data and submit them to the evaluation system. A correctly formatted submission should be a text file with exactly 100000 lines. Each line should correspond to a document from the test data set (the order matters!) and contain a list of one or more predicted labels, separated by commas.

Evaluation: the quality of submissions will be evaluated using the average F1-score measure, i.e., for each test document, the F1-score between the predicted and true labels will be computed, and the values obtained for all test cases will be averaged.

## Usage
The projects is in Jupyter Notebook `abstracts.ipynb` (html version `abstracts.html`).

#### Running and development
```bash
virtualenv --python=python3 venv
source venv/bin/activate
pip install -r requirements.txt
jupyter lab
```
