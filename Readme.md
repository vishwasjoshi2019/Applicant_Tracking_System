## Resume Shortlisting using NLP and KNN

This project showcases a comprehensive approach to automate the resume shortlisting process using Natural Language Processing (NLP) techniques and the K-Nearest Neighbors (KNN) algorithm. The combination of these approaches allows efficient and accurate matching of job descriptions with candidate resumes.

### Process Overview
- Tokenization: Tokenization involves breaking down text into individual words or tokens. This process is crucial for further analysis, as it converts a continuous text into a structured format for manipulation.

- Stemming and Lemmatization: Both stemming and lemmatization aim to reduce words to their base or root forms. Stemming involves removing prefixes or suffixes from words, while lemmatization employs dictionaries to convert words to their base forms.

- Text Preprocessing: This step includes removing non-ASCII characters, converting text to lowercase, eliminating punctuation, and replacing numbers with their English spellings.

- Removing Stopwords: Stopwords are commonly used words like "and," "the," "in," etc., that don't contribute much to the meaning of a sentence. Removing these words helps to focus on content-rich terms.

- Vectorization (TF-IDF): TF-IDF (Term Frequency-Inverse Document Frequency) is a numerical representation of the importance of words in a document relative to a collection of documents. It captures the significance of words within a document compared to their frequency across all documents.

- K-Nearest Neighbors (KNN): KNN is a machine learning algorithm used for classification and regression tasks. In this context, KNN finds the nearest neighbors (similarities) between the vectorized job description and each resume's vector. It calculates the "distance" between vectors and selects the resumes with the closest proximity to the job description.

### Technique Explained
- Tokenization: Tokenization splits text into individual tokens (words or phrases). It helps in creating a structured representation of textual data for further analysis.

- Stemming: Stemming reduces words to their root form. For example, "running," "runner," and "runs" are all stemmed to "run."

- Lemmatization: Lemmatization converts words to their base or dictionary form. For example, "better" and "best" are lemmatized to "good."

- Text Preprocessing: Removing non-ASCII characters ensures compatibility, while converting to lowercase standardizes the text. Removing punctuation enhances readability, and replacing numbers aids in uniform processing.

- Removing Stopwords: We focus on more meaningful terms by eliminating common words, leading to better analysis results.

- TF-IDF Vectorization: TF-IDF assigns weights to words based on their frequency in a document and across documents. It emphasizes important terms while downplaying common ones.

- KNN Algorithm: KNN measures the distance between vectors to find the "nearest neighbors." In this case, the closest resumes to the job description are shortlisted as potential matches.

### How to Run the Code

1. The provided file is an `.ipynb` notebook, designed to run in Jupyter Notebook.
2. Ensure the following packages are installed by running these commands in the Jupyter Notebook:
```python
!pip install nltk
!pip install inflect
!pip install gensim==3.8.3
!pip install PyPDF2
!pip install sklearn

```

3. If any package is missing, install it using similar commands as above.
4. Make the following changes in the code:- Modify the file paths according to your system for the resume folder and the job description.
5. you're ready to run the code after these changes and package installations.
6. Note that some comments within the code for debugging purposes can be ignored.

### Explanation of the Code

The code demonstrates a resume shortlisting process using NLP and KNN techniques. It involves the following steps:

1. **Importing Modules**: Importing required libraries for text processing, PDF extraction, and KNN modeling.

2. **ResultElement Class**: Defines a class to store the final output ranking and filenames.

3. **Preprocessing Functions**: Functions for text preprocessing including removing non-ASCII characters, converting to lowercase, removing punctuation, replacing numbers, removing stopwords, stemming, and lemmatizing.

4. **Normalization Function**: Combines the preprocessing functions to normalize the text.

5. **Parsing Resumes**: Extracts text content from PDF, DOC, and DOCX files, preprocesses the content, and stores it in the `Resumes` list.

6. **Parsing Job Description**: Extracts and summarizes the text content from the job description.

7. **Vectorization and KNN**: Utilizes TF-IDF vectorization to create vectors for both the job description and each resume. KNN is applied to find the nearest neighbors (similarities) between the job description and resumes.

8. **Resume Shortlisting and Result Display**: Displays the shortlisted resumes ranked by similarity to the job description.

Feel free to customize the code according to your needs and use it to streamline the resume shortlisting process based on job descriptions.

## Creator

This project was created by [Vishwas Joshi](https://github.com/vishwasjoshi2019).


[![GitHub](https://img.shields.io/badge/GitHub-%40vishwasjoshi2019-blue)](https://github.com/vishwasjoshi2019)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%40vishwasjoshi2019-blue)](https://www.linkedin.com/in/vishwasjoshi2019/)
[![Gmail](https://img.shields.io/badge/Gmail-vishwasjoshi2019%40gmail.com-red)](mailto:vishwasjoshi2019@gmail.com)
[![Institute Email](https://img.shields.io/badge/Institute%20Email-vishwas.j%40iitgn.ac.in-red)](mailto:vishwas.j@iitgn.ac.in)
[![Instagram](https://img.shields.io/badge/Instagram-%40cursed__geek-orange)](https://www.instagram.com/cursed_geek/)
[![Twitter](https://img.shields.io/badge/Twitter-%40Vishwas79116150-blue)](https://twitter.com/Vishwas79116150)

