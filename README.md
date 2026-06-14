🌸 Iris Flower Classification

My first Machine Learning project — built to understand the end-to-end ML workflow from raw data to model evaluation.

🎯 Objective

Classify Iris flowers into three species — Setosa, Versicolor, or Virginica — based on sepal and petal measurements, using supervised learning.

🛠️ Tech Stack

Python — Jupyter Notebook

Pandas — data loading and manipulation

Matplotlib — visualizations

Scikit-learn — preprocessing, models, evaluation

📊 Dataset

The classic Iris dataset (built into Scikit-learn): 150 samples, 3 classes, 4 features.
Features include Sepal Length (cm), Sepal Width (cm), Petal Length (cm), and Petal Width (cm).

EDA finding: Petal measurements create far cleaner clusters than sepal measurements. Setosa is almost perfectly separable; Versicolor and Virginica overlap slightly.

🧠 Models

K-Nearest Neighbors (K=3) achieved 100% accuracy.
Logistic Regression achieved 100% accuracy.

Both models achieved 100% on the 30-sample test set. This is expected — the Iris dataset is small, clean, and has very distinct class boundaries. Real-world datasets rarely behave this cleanly.

🔬 K-Value Experiment

Tested KNN across every K from 1 to 20 to observe how accuracy changes.

Result: Accuracy held at 100% across all K values.

Why? The dataset's class boundaries are so linearly separable that even a K=20 majority vote never misclassifies. A flat curve here isn't boring — it's informative about the nature of the data.



📝 Key Concepts I Learned

Train/Test Split — Never evaluate on training data. I used 80/20 split with random_state=42 for reproducibility.

StandardScaler — KNN is distance-based, so feature scaling matters. Critical distinction: fit_transform on training data only; transform (no re-fit) on test data. Re-fitting on test data causes data leakage.

Confusion Matrix — Accuracy alone can mislead. The matrix confirmed no off-diagonal errors — the model wasn't accidentally correct.

Model Comparison — Running two algorithms side by side showed that for linearly separable data, a simple Logistic Regression matches a more complex KNN. Model choice matters more on harder problems.

🚀 Run It Yourself

git clone https://github.com/Ira9181/iris-classification.git
cd iris-classification
pip install numpy pandas matplotlib scikit-learn jupyter
jupyter notebook

Open iris.ipynb and run all cells.

📁 Structure

The iris-classification folder contains iris.ipynb (Full notebook — EDA, models, K-value experiment) and README.md.

🔮 What's Next

This project established the pipeline. Next goals: Work with a messier, real-world dataset, explore cross-validation for more robust evaluation, try decision trees and random forests, and start working with unstructured data (text/images).
