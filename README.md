# AUTOCORRECTOR-USING-NLP
Autocorrect feature predicts and correct misspelled words, it helps to save time invested in the editing of articles, emails and reports. This feature is added many websites and social media platforms to ensure easy typing.
You're right — here’s the properly formatted *Markdown file* for README.md — with *correct markdown syntax* and no extra explanation:

markdown


📁 Project Structure



AUTOCORRECTOR-USING-NLP/
├── autocorrector using nlp.ipynb               # Main script to run the autocorrector
├── final.txt            # Word corpus used for building vocabulary
├── LICENSE               # License info (MIT)
└── README.md             # This file

`

## 📄 Prerequisites

- A vocabulary text file (e.g., final.txt) with one or more words per line or paragraph.
- All words should be *lowercase* and *newline-separated*.

---

## 🛠 Usage

### 1. Clone the repository

bash
git clone https://github.com/Shashankkusu/AUTOCORRECTOR-USING-NLP.git
cd AUTOCORRECTOR-USING-NLP
`

### 2. Prepare your dictionary

Use a large text file like sample.txt. Ensure:

* All text is lowercase
* Words are separated by whitespace or newline

### 3. Run the main script

bash
python main.py


This starts a simple prompt. Enter a word to get correction suggestions.

#### Example


Enter a word: tehre
Suggestions: there, their


---

## 🧱 Implementation (Summary)

* main.py:

  * Reads sample.txt, splits words, and builds a word frequency table.
  * Calculates word probabilities using:
    probability = frequency / total word count
  * Defines edit functions:

    * delete_letter()
    * swap_letters()
    * replace_letter()
    * insert_letter()
  * Combines edits to generate candidates within 1 or 2 edits.
  * Ranks candidates based on word probability.
  * Accepts user input interactively.

---

## 📊 Example

bash
$ python main.py
Enter word: exampel
output:
1. example 


---

## 📝 Customization

* *Use your own corpus*: Replace final.txt with a larger dataset.
* *Edit distance*: Adjust the depth of candidate generation (1 or 2 edits).
* *Ranking improvements*: Add bigram context or use n-gram models.
* *Optimize performance*: Use caching or prune low-probability candidates.

---

## 🚀 Improvements & Extensions

* Add *context-aware correction* using n-gram or language models.
* Use *NLTK's tokenizer/lemmatizer* for preprocessing.
* Build a *Flask/Streamlit* UI for web-based usage.
* Test on datasets with known misspellings and analyze accuracy.

---

## 🧪 Testing & Evaluation

Create a test suite test_words.txt with entries like:


tehre → there
recieve → receive




---

## 📄 License

This project is released under the *MIT License*. See [LICENSE](LICENSE) for details.

---

## 🙌 Acknowledgments

* Inspired by Peter Norvig’s “How to Write a Spelling Corrector”.
* Related projects:

  * [filyp/autocorrect](https://github.com/filyp/autocorrect)
  * [gvdnikhil/Autocorrect-Feature-using-NLP-with-Python](https://github.com/gvdnikhil/Autocorrect-Feature-using-NLP-with-Python)
  * [Wanghley/Word-Autocorrection-NLP](https://github.com/Wanghley/Word-Autocorrection-NLP)
* Tutorial reference:

  * [GeeksforGeeks Autocorrector Tutorial](https://www.geeksforgeeks.org/autocorrector-feature-using-nlp-in-python/)

---

## 🤝 Contribution

Feel free to:

* Report bugs via *Issues*
* Suggest features via *Pull Requests*

Your contributions are welcome! 🚀
