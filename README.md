Sentiment Analysis with Multiple Models
Project Overview

This project performs sentiment analysis on text data using classical machine learning models. The objective is to classify text (movie reviews) into Positive or Negative sentiment and compare the performance of Naive Bayes and Support Vector Machine (SVM).

The project follows a research-oriented approach including preprocessing, feature extraction, model training, evaluation, and ablation study.

Objectives
Perform sentiment classification on real-world dataset
Compare Naive Bayes and SVM models
Analyze impact of preprocessing and TF-IDF
Conduct ablation study
Visualize results using graphs and confusion matrix
Project Structure

sentiment-analysis-multiple-models/

data/
dataset_large.csv

src/
preprocess.py
train_models.py
evaluate.py

results/
accuracy_graph.png
confusion_matrix.png

main.py
requirements.txt
README.md
paper.pdf

Dataset
Dataset: IMDB Movie Reviews
Total records: 50,000
Labels: Positive / Negative
Real-world dataset with diverse text
Technologies Used
Python
Pandas
NumPy
Scikit-learn
NLTK
Matplotlib
Workflow
Load dataset
Preprocess text (lowercase, remove punctuation, stopwords)
Convert text into TF-IDF features
Train models (Naive Bayes, SVM)
Evaluate performance
Generate graphs and confusion matrix
Results

Naive Bayes:
Accuracy: 0.84
Precision: 0.83
Recall: 0.82
F1-score: 0.82

SVM:
Accuracy: 0.90
Precision: 0.89
Recall: 0.88
F1-score: 0.88

Conclusion: SVM performs better due to its ability to handle high-dimensional data.

Ablation Study

Without preprocessing: 0.70
CountVectorizer: 0.78
TF-IDF + NB: 0.84
TF-IDF + SVM: 0.90

Insight: Preprocessing and TF-IDF significantly improve performance.

Visual Outputs
Accuracy comparison graph is stored in results/accuracy_graph.png
Confusion matrix is stored in results/confusion_matrix.png
How to Run

Step 1: Clone repository
git clone https://github.com/your-username/sentiment-analysis-multiple-models.git

Step 2: Navigate to folder
cd sentiment-analysis-multiple-models

Step 3: Install dependencies
pip install -r requirements.txt

Step 4: Run the project
python main.py

Requirements

pandas
numpy
scikit-learn
nltk
matplotlib

Research Paper

The project includes a research paper (paper.pdf) with detailed methodology, experiments, and analysis.

Limitations
Cannot handle sarcasm effectively
Limited contextual understanding
Only binary classification
Future Work
Use deep learning models like BERT
Extend to multilingual datasets
Improve sarcasm detection
Build real-time system
Contribution

You can fork this repository and improve the project.

Acknowledgment

IMDB Dataset
Scikit-learn Library
