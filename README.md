## Simple_Information_Retrieval_Project
# Gutenberg Books Search Engine using NLP and TF-IDF

This project aims to develop a simple **Information Retrieval (IR) system** in Python using the **Gutenberg Dataset (15,000 books)**. It leverages NLP libraries such as **spaCy** and **NLTK** for text preprocessing, and employs **TF-IDF** vectorization along with **Cosine Similarity** to rank documents based on user queries. It lists the top 10 most relevant books, ranked and scored according to their similarity to the query. In addition, it features a basic **Boolean Retrieval** model and supports comprehensive performance evaluation using **Precision**, **Recall**, and **F1-Score**.

---

## Dataset

The dataset is downloaded from Kaggle via [kagglehub](https://www.kaggle.com/datasets/mateibejan/15000-gutenberg-books) and contains metadata such as:
- Title
- Author
- Link
- Bookshelf category

---

##  Features

-  Text preprocessing (tokenization, stemming, stopword removal)
-  Inverted Index creation
-  Boolean Retrieval (AND query support)
-  TF-IDF calculation
-  Cosine Similarity for ranking
-  Boolean Matrix generation
-  Evaluation: Precision, Recall, F1-Score, AP, MAP

---

##  How to Run

1. **Clone the repository**:
```bash
git clone https://github.com/yourusername/gutenberg-search-engine.git
cd gutenberg-search-engine
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Run in Google Colab** or locally in Jupyter Notebook.

---

##  Dependencies

The required packages are listed in `requirements.txt`:
Also run the following after installation:

```bash
python -m spacy download en_core_web_sm
```
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('popular')
```

---

## Evaluation Metrics

- **Precision**: Relevant documents among retrieved ones
- **Recall**: Retrieved relevant documents among all relevant ones
- **F1-Score**: Harmonic mean of precision and recall
- **Average Precision (AP)**: Ranked relevance score


---

## Example Query

Example query:  
```
wild animal home
```

Sample output:
```
1. Wild Animals at Home
2. Wild Animals I Have Known
3. The Minds and Manners of Wild Animals: ...
```

---

## License

This project is open-source
