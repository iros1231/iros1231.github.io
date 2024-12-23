---
title: Duar N-Max
author: Duar
tags:
  - duar
  - medicine
  - big data
---

<!-- excerpt start -->
Most machine learning algorithms are fulfilled with mathematical things such as statistics, algebra, calculus and etc. They expect the data to be numerical such as a 2-dimensional array with rows as instances and columns as features. The problem with natural language is that the data is in the form of raw text, so that the text needs to be transformed into a vector. The process of transforming text into a vector is commonly referred to as text vectorization. It’s a fundamental process in natural language processing because none of the machine learning algorithms understand a text, not even computers. Text vectorization algorithm namely TF-IDF vectorizer, which is a very popular approach for traditional machine learning algorithms can help in transforming text into vectors.
<!-- excerpt end -->

### TF-IDF
Term frequency-inverse document frequency is a text vectorizer that transforms the text into a usable vector. It combines 2 concepts, Term Frequency (TF) and Document Frequency (DF).

The term frequency is the number of occurrences of a specific term in a document. Term frequency indicates how important a specific term in a document. Term frequency represents every text from the data as a matrix whose rows are the number of documents and columns are the number of distinct terms throughout all documents.
Document frequency is the number of documents containing a specific term. Document frequency indicates how common the term is.

Inverse document frequency (IDF) is the weight of a term, it aims to reduce the weight of a term if the term’s occurrences are scattered throughout all the documents. IDF can be calculated as follow:
Display equation: $${idf}_i=\log(\dfrac{n}{{df}_i})$$
Where idfᵢ is the IDF score for term i, dfᵢ is the number of documents containing term i, and n is the total number of documents. The higher the DF of a term, the lower the IDF for the term. When the number of DF is equal to n which means that the term appears in all documents, the IDF will be zero, since log(1) is zero, when in doubt just put this term in the stopword list because it doesn't provide much information.

The TF-IDF score as the name suggests is just a multiplication of the term frequency matrix with its IDF, it can be calculated as follow:
Inline equation: $w_i,j={tf}_i,j \times {idf}_i$

Where wᵢⱼ is TF-IDF score for term i in document j, tfᵢⱼ is term frequency for term i in document j, and idfᵢ is IDF score for term i.
