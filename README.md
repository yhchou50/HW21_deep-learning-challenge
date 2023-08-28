# HW21_deep-learning-challenge

1.Overview of the Analysis: Explain the Purpose of this Analysis 

The nonprofit foundation Alphabet Soup requires a tool to aid in selecting funding applicants with the highest likelihood of success in their ventures. Leveraging your expertise in machine learning and neural networks, your task is to utilize the features within the provided dataset to develop a binary classifier. This classifier should predict whether applicants will achieve success if funded by Alphabet Soup.

2. Results: Address the Following Questions Using Bulleted Lists and Images for Support

Data Preprocessing

What is the target variable for your model?

Answer: The target variable (y) is the "IS_SUCCESSFUL" feature (column).
What are the features for your model?

Answer: Initially, there were 11 features/columns in the original dataset, excluding "IS_SUCCESSFUL." By establishing cutoff points for "application_type" and "classification" and utilizing the "get_dummies()" function to convert categorical data into numeric, the dataset was expanded to include 47 features. Subsequently, I lowered the cutoff to generate additional features for optimization purposes (attempt-3, refer to starter_code_3), resulting in 117 features.
Which variables should be excluded from the input data as they are neither targets nor features?

Answer: "ID" and applicant names were removed, leaving 9 features for the model.
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you choose for your neural network model, and why?

Answer: The goal was to achieve accuracy above 75%. In my initial attempt (attempt-1), I used two hidden layers with 6 neurons each, and trained for 100 epochs. This yielded an accuracy of 72.52%. Refer to the image in the "Starter_code.ipynb" file. For the second attempt, I increased the neuron count to 30 and 15 for the first and second hidden layers respectively. Despite training for 100 epochs, the accuracy only improved slightly to 72.56%, not significantly different from attempt-1. In the third attempt (Starter_code-3), I introduced an additional hidden layer and extended the number of epochs to 200. This resulted in a slight accuracy boost to 72.69%, though the improvement remained marginal.
Did you achieve the target model performance?

Answer: No.
What steps did you take to enhance model performance?

Answer: I believe there's still potential for refining the data size and processing. Standardizing the "ask_amount" could be beneficial. Additionally, experimenting with increased layers, neurons, and different activation functions will be explored in forthcoming optimization attempts.

