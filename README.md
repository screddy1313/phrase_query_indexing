# phrase_query_indexing
In this project we construct phrase query retrieval using 20_newsgropus dataset

## Getting Started
Before running the above code please make sure that, you have downloaded 20_newsgroups dataset which is freely available in the internet and place in the data folder.
Now run the code cell by cell.

### Installing
The following packages are used for the project
```
+ python 3
+ nltk for text processing
+ pickle for storing and loading data structures
```
### Pre processing
```
+ Removal of meta data in each file
+ Removal of symbols like [!@#$%^&*()] from the tokens
+ Removal of non alpha numeric tokens
+ Lemmatization of tokens
+ Removal of words that are less than size 2 (useless words)
```
### Methodology 
+ Positional Indexing is constructed for two folders *rec.motorcycles*, *comp.graphics* in 20_newsgroups dataset
+ Preprocessing each file in the above folders
+ Construction of the positional indexing dictionary. (Code is self explainatory with comments)
+ when the user gives the query, we find the relative distance between tokens in the query and retrieve all the files which contains tokens in the same distance.

### References 

followed chris manning book for constructing the dictionary [link](https://nlp.stanford.edu/IR-book/pdf/03dict.pdf)
