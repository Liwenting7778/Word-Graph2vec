# Word-Graph2vec
Word Graph2vec is a graph based word embedding algorithm that converts a large corpus into a word co-occurrence graph, randomly selects word sequence samples, and embeds words into the sampled corpus for training. We assume that due to the limited vocabulary, large number of idioms, and fixed expressions in English, the size and density of word co-occurrence maps will slightly change with the increase of the training corpus. Therefore, WordGraph2vec has stable runtime on large-scale datasets, and its performance advantage becomes increasingly evident as the training corpus grows. See more details in the paper:[Word-Graph2vec: An Efficient Word Embedding Approach on Word Co-occurrence Graph Using Random Walk Technique](https://link.springer.com/chapter/10.1007/978-981-99-7254-8_68)


# Requirements
The codebase is implemented in Python 3.8 package versions.

    ```python
    pip install -r requirements.txt 
    ```

# Datasets  
We use various data sets to test our approaches. The processed dataset information can be found in Table 1.
[Text8](http://mattmahoney.NET/dc/text8.zip): Text8 contains 100M processed Wikipedia characters created by changing the case to lower of the text and removing any character other than the 26 letters a through z. Meanwhile, PyDictonary, as in the English language dictionary, Wordnet lexical database, and Enchant Spell Dictionary, is applied to filter the correct English words.
One billion words benchmark ([1b words banchmark](https://www.kaggle.com/datasets/alexrenz/one-billion-words-benchmark): This is a new benchmark corpus with nearly 1 billion words of training data, which is used to measure the progress of statistical language modeling.
Enlish Wikipedia data set ([En-Wikipedia](https://dumps.wikimedia.org/enwiki/latest/enwiki-latest-pages-articles.xml.bz2): This is a word corpus of English articles collected from Wikipedia web pages.

<img width="348" alt="image" src="https://github.com/Liwenting7778/Word-Graph2vec/assets/93420681/40272ea8-7448-4ec1-b3f0-a5d462b3e731">




# Evaluation
In the experiment, we used the following methods to evaluate the quality of word vectors:[word-embeddings-benchmarks](https://github.com/kudkudak/word-embeddings-benchmarks)
