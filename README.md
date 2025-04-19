# deep-learning-challenge

This repository contains my submission for the Deep Learning Challenge. In the repository you will find 4 files, my initial model and 3 optimizations. The goal of these optimizations are to achieve model accuracy higher than .75. These ipynb files are intended to be ran in Google Colab.

# Deep Learning Challenge Report

Overview of Analysis: The purpose of this analysis is to evaluate model performance and provide recommendations for further optimization.

Results:

Data Preprossessing:
- The target for the model is the "IS_SUCCESSFUL" column.
- The features of the model are the "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT"columns.
- The variables that could be removed are "EIN" and "NAME".

Compiling, Training, and Evaluating the Model:
- For the first model, I used 2 hidden layers with 16 neurons in the first and 5 in the second. The activation function for the first two layers was ReLU with Sigmoid being used for the output layer. I did this based on previous practice and determined it to be a good baseline.
- My model did not achieve target performance. Initial model: Accuracy = 72.6%, Loss = 0.56.
- In my attempts to increase model performance, I added additional layers, additional neurons, and increased the number of epochs. 
- Optimized Model One: In this optimization, I updated the first hidden layer to have 80 neurons and the second to have 30. This only slightly improved model performance. Optimized Model One: Accuracy = 72.9%, Loss = 0.57.
- Optimized Model Two: In this optimization, I added an additional hidden layer with 10 neurons and a ReLU activation function. This had a minimal effect on model performance.Optimized Model Two: Accuracy = 72.9%, Loss = 0.56.
- Optimized Model Three: In this optimization I added another hidden layer and updated neurons to be, in order of layers, 128, 62, 32, and 16. This caused the model to perform sligthly worse. Optimized Model Three: Accuracy = 72.7%, Loss = 0.57.


![Model Loss Over Epochs](https://github.com/user-attachments/assets/cbbe9200-3118-4548-9882-c935e2ab0090)

![Model Accuracy Over Epochs](https://github.com/user-attachments/assets/980c9ed4-2e76-4a71-a898-aefe2eaa5afc)


Summary: Overall, the model and my 3 attempts at optimization did not achieve the target performance. I chose the optimizations I did based on my understanding of what we learned in class, but now that I've had more practice I can recognize additional opportunities for improvement. For a different model, I'd recommend further increasing hidden layers, increasing the number of values in the bins, and adding more epochs. I also believe that adding back in one or both of the columns removed would increase model performance.I believe that this would increase model performance.

Additionally, an alternative model that could be beneficial to use would be a Rendom Forest Classifier. This data set includes several categorical vairables, so based on my research, Random Forest might be more interperatable and faster to tune when compared to a neural network.
