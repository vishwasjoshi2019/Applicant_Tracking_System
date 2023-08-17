## Resume Shortlisting using NLP and KNN

This project demonstrates an approach to shortlist resumes based on a provided job description using Natural Language Processing (NLP) techniques and the K-Nearest Neighbors (KNN) algorithm.

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
6. Note that there are some comments within the code for debugging purposes, which can be ignored.

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

