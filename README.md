# Clinical-Notes
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

