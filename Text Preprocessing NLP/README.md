# NLP Text Preprocessing Pipeline

This project demonstrates a step-by-step Natural Language Processing (NLP) preprocessing workflow built in Python using regular expressions, NLTK, and spaCy. It was created as a class assignment to show how raw text can be transformed into cleaner, structured input for downstream NLP or machine learning tasks.

## Project Overview

The notebook processes a sample paragraph containing common real-world text issues such as:

- URLs
- Hashtags
- Punctuation
- Numbers
- Mixed casing
- Stopwords
- Noisy user-generated text

The pipeline then applies a sequence of preprocessing steps and prints the output after each stage so the transformation is easy to follow.

## Objectives

- Build a complete NLP preprocessing pipeline from raw text.
- Understand how text changes after each cleaning step.
- Practice using Python libraries commonly used in NLP.
- Prepare text for machine learning or text analytics tasks.

## Workflow Implemented

The notebook includes the following preprocessing stages:

1. **Raw text input**  
   A multi-line paragraph is used as the source text. It includes URLs, hashtags, punctuation, numbers, and mixed formatting.

2. **Text cleaning with regular expressions**  
   The script removes:
   - URLs using `re.sub(r'http\\S+', '', text)`
   - Hashtags using `re.sub(r'#\\w+', '', clean_text)`
   - Non-alphabetic characters such as punctuation, numbers, and emojis using `re.sub(r'[^A-Za-z\\s]', ' ', clean_text)`

3. **Lowercasing**  
   All text is converted to lowercase to standardize token matching.

4. **Tokenization**  
   The cleaned text is split into individual word tokens using NLTK's `word_tokenize()`.

5. **Stopword removal**  
   Common English stopwords are removed using `nltk.corpus.stopwords`.

6. **Lemmatization**  
   Tokens are reduced to their base form using spaCy (`en_core_web_sm`).

7. **Final preprocessed text generation**  
   The lemmatized tokens are joined back into a single processed text string.

## Technologies Used

- **Python**
- **re** for pattern-based text cleaning
- **NLTK** for tokenization and stopword removal
- **spaCy** for lemmatization
- **Jupyter Notebook** for interactive execution

## File Structure

```bash
.
├── Text_Preprocessing_Pipeline_NLP.ipynb
└── README.md
```

## Example Concepts Covered

This project helps demonstrate practical preprocessing concepts used in:

- Sentiment analysis
- Text classification
- Chatbots
- Search and retrieval systems
- Social media text analysis
- Customer feedback mining

## Key Learning Takeaways

- Text preprocessing is essential before training NLP models.
- Each preprocessing step affects meaning and model quality.
- Blindly removing words such as `not` can change sentence meaning.
- Hashtags and other social text patterns may carry useful contextual information.
- Combining regex, NLTK, and spaCy creates a simple but effective preprocessing workflow.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/<your-repository-name>.git
cd <your-repository-name>
```

2. Install the required libraries:

```bash
pip install nltk spacy notebook
```

3. Download the required NLP resources:

```bash
python -m nltk.downloader punkt stopwords
python -m spacy download en_core_web_sm
```

4. Launch Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `Text_Preprocessing_Pipeline_NLP.ipynb` and run the cells.
