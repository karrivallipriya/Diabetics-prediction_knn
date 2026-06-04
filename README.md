I'm a 3rd year ECE student and I built this while exploring ML for the first time. Followed along with a GeeksForGeeks tutorial and made sure I understood every single line before documenting it.

**What I learned**

Before this project, I had only theoretical knowledge of ML. Actually coding it end-to-end helped me understand why each step matters — why we scale data, why we split into train/test, and why accuracy alone isn't enough to evaluate a model. Every cell in the notebook has a comment explaining what that code does and why.


**What I did**

I started with **Exploratory Data Analysis (EDA)** to get familiar with the data — checking for missing values, duplicates, and understanding what each column means. Then I used **Seaborn and Matplotlib** to visualize things like class balance, outliers, feature distributions, and how correlated the features are with each other. One thing I noticed is that Glucose and BMI had the strongest relationship with the diabetic outcome.
After that, I preprocessed the data using **StandardScaler** to normalize all the features. This step is important because **KNN is a distance-based algorithm** — if one feature has a much larger range than others, it will dominate the distance calculation and mess up the predictions.
For the model, I used K-Nearest Neighbors (KNN). I tried different values of K from 1 to 14 and plotted the train and test accuracy for each to find the best one. K=13 gave the most balanced result. Finally, I evaluated the model using a confusion matrix and classification report to check precision, recall, and F1-score — not just overall accuracy.


**Dataset and credits**

**Dataset: Pima Indians Diabetes Database — UCI ML Repository via Kaggle**
I followed along with the **GeeksForGeeks ML projects series on YouTube** to build this. All the explanations in the notebook are written by me after understanding the code.

**How to run it**

Open the .ipynb file in Jupyter Notebook, VS Code, or Google Colab. If you're running it locally, just change the dataset path to wherever you saved the CSV file and run all cells in order.

THANK YOU!
