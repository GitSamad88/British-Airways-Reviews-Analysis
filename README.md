# British Airways Reviews Analysis

This project analyses British Airways customer reviews to explore sentiment, identify recurring themes, and generate insights from unstructured text data.

## Project overview

The workflow is split across notebooks:

- `notebooks/BA reviews collection & cleaning.ipynb` - collects and prepares the raw review data
- `notebooks/BA reviews EDA and Sentiment Analysis.ipynb` - performs exploratory data analysis, sentiment analysis, and topic modelling

## Folder structure

```text
BA reviews project/
├── data/
│   └── BA_reviews.csv
├── notebooks/
│   ├── BA reviews collection & cleaning.ipynb
│   └── BA reviews EDA and Sentiment Analysis.ipynb
├── outputs/
│   └── BA_reviews_sentiment_analysis.csv
├── README.md
├── requirements.txt
└── .venv/  (optional local virtual environment)
```

## Setup

1. Create a virtual environment:

```bash
python -m venv .venv
```

2. Activate it:

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

On Windows Command Prompt:

```cmd
.venv\Scripts\activate.bat
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Download NLTK stopwords if prompted by the notebook:

```python
import nltk
nltk.download('stopwords')
```

## Running the notebooks

Open the notebooks in Jupyter Notebook or VS Code and run cells in order:

```bash
jupyter notebook
```

## Main analysis goals

- understand rating distribution
- identify common review themes
- compare positive vs negative review language
- perform sentiment analysis
- apply topic modelling to discover hidden themes

## Output

The final enriched dataset is saved in the `outputs/` folder as:

- `BA_reviews_sentiment_analysis.csv`

## Requirements summary

This project uses:

- Python 3.10+
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn
- nltk
- wordcloud

## Notes

The notebooks assume the cleaned CSV is available at:

```text
data/clean_BA_reviews.csv
```

If the file name differs in your environment, update the file path in the notebook before running it.
