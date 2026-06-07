🌸 Iris Flower Classification

My very first Machine Learning project! I built this to get hands-on experience with the end-to-end ML workflow—from loading data and visualizing it, to training models and making predictions.

🎯 The Goal
Classify Iris flowers into three species (Setosa, Versicolor, or Virginica) based on their sepal and petal measurements using Supervised Learning.

🛠️ Tools Used
Python 
Jupyter Notebook
Pandas (Data manipulation)
Matplotlib (Data visualization)
Scikit-learn (ML models & preprocessing)

📊 The Dataset
Used the classic Iris dataset (built into Scikit-learn). It contains 150 flowers with 4 features:
Sepal length & width (cm)
Petal length & width (cm)

Visualizing the data showed that petal measurements create very clear clusters, making them great predictors for the species.

🧠 Models Built & Results
I trained two different classification models to compare them:

1. K-Nearest Neighbors (KNN) — n_neighbors=3
2. Logistic Regression — max_iter=200

Results
Both models achieved 100% accuracy on the test set (30 flowers). The confusion matrix showed perfect predictions across all three species. 

Note: 100% accuracy is achievable here because the Iris dataset is small and very clean with distinct class boundaries. In real-world datasets, 80-90% is usually considered excellent!

📝 What I Learned
By building this project from scratch, I learned the foundational pipeline that every ML project follows:

Data Exploration: How to load, inspect, and plot data to find patterns before modeling.
Train/Test Split: Why it's crucial to hide a portion of data from the model during training to evaluate it fairly.
Feature Scaling: How to use StandardScaler to normalize data, and the critical difference between fit_transform (training data) and transform (test data).
Model Evaluation: How to read a Confusion Matrix and why accuracy isn't the only metric that matters.
Prediction: How to pass brand-new data into a trained model and interpret prediction probabilities.

🚀 How to Run
1. Clone the repo
git clone https://github.com/Ira9181/iris-classification.git

2. Install the required libraries
pip install numpy pandas matplotlib scikit-learn jupyter

3. Launch Jupyter Notebook
jupyter notebook

4. Open the .ipynb file and run the cells!
