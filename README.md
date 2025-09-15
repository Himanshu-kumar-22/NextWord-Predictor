# Next Word Predictor

This project implements a **Next Word Prediction model** using Recurrent Neural Networks (LSTMs/GRUs).  
The goal is to predict the most likely next word given a sequence of words, similar to how modern keyboards provide text suggestions.

---

## 📂 Dataset

We use the **WikiText-103** dataset, which contains over 100 million words extracted from Wikipedia.  
Dataset link: [WikiText-103](https://www.kaggle.com/datasets/rohitgr/wikitext)  

Files used:  
- `wiki.train.tokens` (training data)  
- `wiki.valid.tokens` (validation data)  
- `wiki.test.tokens` (test data)  

> ⚠️ Note: The dataset files are not uploaded in this repository (too large). Please download them from the official source.

---

## ⚙️ Installation

Clone this repository:

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

Install dependencies:
pip install -r requirements.txt

Run the Jupyter notebook:
jupyter notebook nextword.ipynb

📊 Performance
	•	Training dataset size (sentences): ~35,000
	•	Evaluation metric: Perplexity (standard for language modeling)
	•	Test Perplexity: 114

	![Performance Snapshot]('metrics.png')

📌 Future Improvements
	•	Add Transformer-based models (BERT/Transformer Decoder) for comparison
	•	Hyperparameter tuning for better accuracy
	•	Deploy as a web demo (Flask/Streamlit)