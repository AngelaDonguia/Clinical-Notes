# Notice

This repository holds an attempt to finding all the notes by the clinical team, and providing sequencing and analysis of the data from the feedback. This data is obtained from [NBME - Score Clinical Patient](https://www.kaggle.com/competitions/nbme-score-clinical-patient-notes) Notes, a kaggle challenge.

# Overview

This notebook is used to find out the following:

- Analysing the dataset to find out basic information of the CSV files
- Listing out Sample notes and their corresponding labels with locations
- Visualising the data for patients and their distribution
- Finding out the list of all annotations in the dataset

# Summary of Work Done

The main goal was to find how doctors can easily find out the symptoms of the patients through the use of this notebook and spacy can be used to mark up the annotations with accuracy, such that the doctors don't need to manually annotate the data.

## Table of Contents

### Data

Input files that are used to find and analyse the data includes:
| File Name | Description | Data Size |
| --- | --- | --- |
| features.csv | This is the dataset that contains the features of the patients. | 143 |
| patient_notes.csv | This is the dataset that contains the notes of the patients. | 295010 |
| train.csv| Has a comprehensive list of all the notes and their corresponding labels | 14300 |
| test.csv |Has a list of all the notes that are not labelled | 5 |
| sample_submission.csv |Has a list of all the notes that are not labelled | 5|

### Preprocessing / Clean up

Since there was no missing values in the dataset, no cleaning was required.

### Data Visualization

For Data Visulization, SNS was used to plot the following:

- Patient Notes Distribution (Per case)
- Patient Notes Length Distribution
- Feature Distribution (per Case)
- Feature Length Distribution
- Graphing Annotations Distribution
- Annotation Length Distribution

### Problem Formulation

- At first step, we firstly inputted all the csv files to have basic information about the dataset.

- Soon after that, we visualized the data so we can see the frequency of each annotation and how each annotation varies.

- - Such as, how many patients have the annotation, what is the length, are there multiple annotations, etc.

- Later on, we started to find out about how the annotation and patient histroy looks like so we can better understand the data.

- With the previous step out of the way, we visualized all the annotations and their corresponding labels to find frequency and distribution and get the length of ditribution.

- In the end, we highlighted the annotations using Spacy

# How to reproduce results

In this section, provide instructions at least one of the following:

- Reproduce your results fully, including training.
- Apply this package to other data. For example, how to use the model you trained.
- Use this package to perform their own study.

Also describe what resources to use for this package, if appropirate. For example, point them to Collab and TPUs.

# Overview of Files in Repo

**NoteBook File**

- nbme-notes.ipynb

**CSV Files**

- features.csv
- patient_notes.csv
- sample_submission.csv
- test.csv
- train.csv

## Software Setup

**Packages Used**

- warnings
- numpy
- pandas
- seaborn
- matplotlib.pyplot
- random

**How To Install**

```
# Command 1
>>> pip install numpy pandas seaborn matplotlib spacy

# Command 2
>>> py -m spacy download en_core_web_sm
```

## Data

Data can be downloaded from [NBME - Score Clinical Patient](https://www.kaggle.com/competitions/nbme-score-clinical-patient-notes/data)

- Note: For users who are not signed up for the competition would require to sign up for the competition to download the data.

If you have Kaggle API, you can directly use the command:

`kaggle competitions download -c nbme-score-clinical-patient-notes`

## Citations

Some of the references that are used to make this notebook includes:

- https://www.kaggle.com/code/maximilianoalarcon/nbme-score-clinical-patient-notes
- https://www.kaggle.com/code/bhaveshkumar2806/score-clinical-patient-notes-eda-with-plotly
- https://www.kaggle.com/code/ammarabbasi1040/nbme-eda-made-simple
