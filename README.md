# deep-learning-challenge

This repository contains my submission for the Deep Learning Challenge. In the repository you will find 4 files, my initial model and 3 optimizations. The goal of these optimizations are to achieve model accuracy higher than .75. These ipynb files are intended to be ran in Google Colab.

# Deep Learning Challenge Report

Overview of Analysis: The purpose of this analysis is to evaluate model performance and provide recommendations for futher optimization.

Results:

Data Preprossessing:
- The target for the model is the "IS_SUCCESSFUL" column.
- The features of the model are the "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT"columns.
- The variables that could be removed are "EIN" and "NAME".

Compiling, Training, and Evaluating the Model:
- For the first model, I used 2 neurons, 3 layers, and 2 activation functions. I did this based on previous practice and determined it to be a good baseline.
- My model did not achieve target performance.
- In my attempts to increase model performance, I added additional layers, additional neurons, and increased the number of epochs.

Summary: Overall, the model and my 3 attempts at optimization did not achieve the target performance. For a different model, I'd recommend further increaseing hidden layers, increasing the number of values in the bins, and adding more epochs. I believe that this would increase model performance.
