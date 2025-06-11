# OIBSIP_domain_taskno.4
📌 Objective
Build a machine-learning-based spam detector from the ground up using Python and NLP techniques. The goal is to classify SMS messages as "spam" or "ham" (non-spam) by implementing key preprocessing, feature engineering, and classification steps on the SMS Spam Collection Dataset 

🔍 Steps Performed
Data Loading & Cleaning

Imported the SMS Spam Collection Dataset.

Removed unnecessary columns and renamed v1 → label, v2 → message.

Converted labels: spam → 1, ham → 0.

Train-Test Split

Randomly split data into training (≈75%) and testing (≈25%) sets.

Exploratory Data Analysis

Generated WordCloud visualizations highlighting common spam terms (e.g., “FREE”, “claim”, “prize”) versus typical ham terms.

Text Preprocessing

Lowercased messages.

Tokenized text using NLTK.

Performed stemming with Porter Stemmer.

Removed stop words to reduce noise.

Feature Extraction

Implemented two approaches:

Bag of Words (BoW): Counts term frequencies.

TF‑IDF: Weighs words by their frequency and overall importance.

Probability Smoothing

Applied additive (Laplace) smoothing to handle words not seen in training, ensuring non-zero probabilities.

Naïve Bayes Classification

For each message, calculated the probability of being spam vs ham by multiplying feature probabilities with class priors and choosing the higher total.

🛠️ Tools & Libraries Used
Python ecosystem: pandas, NumPy, matplotlib, WordCloud

NLTK: for tokenization, stop-words removal, and stemming

Custom implementation: built Bag‑of‑Words and TF‑IDF feature extractors and a Naïve Bayes classifier from scratch.

✅ Outcome
A working pipeline that preprocesses SMS text and classifies messages with decent accuracy.

Demonstrated the practical difference between BoW and TF‑IDF in classification performance.

Built full NLP model—from raw text to spam detection—without relying on external ML libraries (e.g., scikit-learn), illustrating foundational concepts in text classification.

🧭 How to Use
Clone or download the notebook.

Install required Python libraries (pandas, nltk, etc.).

Run each section sequentially to:

Visualize data

Train classifiers

Evaluate accuracy on the test set

Optionally, feed in your own SMS text to test real-time classification.

🚀 Conclusion
This notebook provides a clear, step-by-step introduction to building an NLP-based spam filter. It covers data wrangling, visualization, basic feature engineering (BoW, TF‑IDF), and the implementation of a Naïve Bayes classifier—all from scratch—making it a solid educational resource for beginners in natural language processing and machine learning.
