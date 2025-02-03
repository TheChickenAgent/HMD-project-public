# Human-Machine Dialogue project

GitHub repository to manage the UniTrento course project for "Human-Machine Dialogue (145864)"

## Description of the project
This project (code and report) is used to evaluate the course. The project is about putting all the concepts from the course into practice and make a Human-Dialogue system for a topic of your choice based on Llama-3. The system in this repository is a food ordering system for a restaurant specialized in chicken.

### Setup of this repository
This repository is set up in the following way:
- notebooks folder: the folder with the running notebooks. There are two versions: one with a segmenter and one without. The version with a segmenter (containing "SEG" in the name) can handle overinformative users better because of the segmenter. Version 5 (```HMD chicken V5 SEG FINAL.ipynb```) was developed after the analysis of the intrinsic evaluation.
- data generation folder: this folder contains the notebooks for data generation for evaluation of the Natural Language Understanding (NLU) component, and Dialogue Manager (DM).
  - P1: NLU prompt without few-shots.
  - P2: NLU prompt with few-shots.
  - P3: NLU prompt to first do intent, than uses different prompts depending on the intent.
- extrinsic evaluation folder: this folder contains the questionnaire and copies of the results.
- The ```Restaurant ROASTED menu.pdf``` file contains the menu card of the restaurant (i.e. the allowed options).
- The report in ```HMD project report.pdf```.

## Installation
The development of this project mainly happend on Kaggle because of the Graphical Processing Unit (GPU) needed to speed up the Large Language Model (LLM). 
Therefore, there is a ```requirements_kaggle.txt``` file which contains the Kaggle packages. THe development was done on Python 3.10.12. There is also a ```pyproject.toml``` file which was manually created and imported all the necessary dependencies from the imports that were used in the notebooks, but this was done in Python 3.10.11

Please note for the use of Llama-3, you need to get an access with, for example, HuggingFace.