# 🧠 E-Commerce Product Classification using Bag of Words (BoW) + Machine Learning

This project performs **multi-class text classification** on an **e-commerce dataset** to classify product categories using **Bag of Words (BoW)** and **Machine Learning**. The classification is done using the **Multinomial Naive Bayes** model, with text preprocessed and vectorized into n-grams (unigrams, bigrams, and trigrams) for better performance.

---

## 🔧 Technologies Used

- Python  
- scikit-learn  
- pandas  
- joblib  
- spaCy  
- Jupyter Notebook  
- CountVectorizer (from scikit-learn)  
- Multinomial Naive Bayes (from scikit-learn)  
- Pipeline (from scikit-learn)

---

## 📁 Dataset

The dataset contains **product names** from various categories, which are classified into 4 categories:

- **Books**  
- **Clothing_Accessories**  
- **Electronics**  
- **Household**  

📌 The raw data was preprocessed in a separate notebook: `ecommerceDataset.ipynb`

### ✨ Preprocessing Steps with spaCy:
- Lemmatization  
- Stopword removal  
- Punctuation removal  
- Lowercasing  

Resulting in a clean dataset: `processed_ecommerceDataset.csv`, ready for model training.

📥 **Dataset Link:** [Download the dataset](https://www.kaggle.com/datasets/saurabhshahane/ecommerce-text-classification)


---

## 📌 Key Features

- **Bag of Words (BoW)** technique for text vectorization.
- Text preprocessed by removing stopwords and normalizing the product names.
- Multiple model attempts tested with different n-grams (unigrams, bigrams, and trigrams).
- **Multinomial Naive Bayes** used for classification.

---

## ✅ Results & Observations

- Achieved **~95% accuracy** on the test data.
- **Unigrams + Bigrams (Attempt 2)** provided the best F1-Score of **0.9516**.
- The model was saved as a **`.pkl` file** for future use.

---

## 📁 Project Files & Folders Explained

| File/Folder | Description |
|-------------|-------------|
| `ecommerceDataset.ipynb` | Notebook for preprocessing the raw dataset using spaCy. |
| `boW_ecommerceDataset.ipynb` | Main notebook for model training, evaluation, and selection. |
| `README.md` | Project overview and usage instructions. |

---

## 🤖 Model Comparison

| Attempt                    | Features Used                    | F1-Score |
|---------------------------|----------------------------------|----------|
| Attempt 1 (1,1)           | Unigrams Only                    | 0.95     |
| Attempt 2 (1,2)           | Unigrams + Bigrams               | **0.95** (Best) |
| Attempt 3 (2,2)           | Bigrams Only                     | 0.94   |
| Attempt 4 (1,3)           | Unigrams + Bigrams + Trigrams    | 0.95   |

---

## 🙌 Credits

🤖Project by **Yahan Madhuhansa**  
This project demonstrates the application of Bag of Words and machine learning for text classification in the domain of e-commerce products.  
Inspired by traditional text classification tasks and the potential of ML models for automatic text categorization.

