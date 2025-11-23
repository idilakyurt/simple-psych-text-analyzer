# Simple Psychological Text Analyzer

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange)

Psychological Rationale & Project Goal
This project is my first attempt to create a code that introduces basic tool related to  **Computational Psychology** and **Natural Language Processing (NLP)**.

As we know, our words do matter and the amount of emotionally charged words can dictate if we have a positive or a negative tone. The core goal is to assess that by using a straightforward **lexical approach**. The method mirrors initial, fundamental steps in psychological data analysis by creating specialized dictionaries (word lists) and tallying word frequencies to infer emotional states. 

The analyzer quantifies the presence of words related to two simple tones: **Positive** and **Negative**.

## 💻 Technical Overview

This notebook (`simple-psych-text-analyzer.ipynb`) demonstrates the essential steps of text processing:

1.  **Lexical Dictionaries:** Defined custom lists of words representing 'Positive' and 'Negative' categories.
2.  **Preprocessing:** The raw text is cleaned by:
    * Converting all characters to **lowercase** (e.g., "Happy" becomes "happy").
    * Removing **punctuation** (`!`, `,`, `.`).
    * **Tokenizing** the text (splitting the text string into a list of individual words).
3.  **Scoring Logic:** A **`for` loop** iterates through every word in the tokenized list. **`if/elif`** conditional statements check for word membership in the positive or negative lists, incrementing the corresponding score.
4.  **Reporting:** The final counts are compared to provide a simple interpretation of the overall tone.

##  How to Run the Analysis

This project was built and run in a Jupyter/Colab Notebook, which is the standard environment for data science projects.

* **View/Run in Google Colab:** (https://colab.research.google.com/drive/1MAL0lPSjHmorHSOF8kGj5KJE12YDcnNE?authuser=0&hl=en#scrollTo=_G6S08B54ibq)
* **To Customize:** The user can easily modify the `sample_text` variable in Step 2 of the notebook or expand the `positive_words` and `negative_words` lists in Step 1 to improve the analysis quality.

## 💡 Future Work (Next Steps in NLP)

To evolve this project toward a more advanced research tool, future steps would include:

* **Using Professional Lexicons:** Integrating validated, larger word sets (e.g., LIWC, VADER) rather than custom lists.
* **Handling Negation:** Developing logic to account for words like "not" (e.g., "I am **not** happy" should not count as a positive word).
* **Visualization:** Adding simple charts (histograms, bar plots) to visually represent the scores, a key component of effective data analysis.
