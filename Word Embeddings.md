# Vector Embeddings

## **What**

Vector embeddings are a way to convert words and sentences and other data into numbers that capture their meaning and relationships.

Words & Sentences (or any data) -> numbers that capture meaning & relationship

We represent the data as points in multidimensional space, where similar data points are clustered closer together. These transformed numbers represent the data itself and help m∫achine to process and understand the data more effectively.

Most common types of vector embeddings are word and sentence embeddings. 

Word embedding creates a high-dimensional space where each word is assigned a dense vector (more on this below) of numbers. A computer can then use these vectors to understand the relationships between words and make predictions.

Word embedding works in natural language processing by representing words as dense vectors of real numbers in a high-dimensional space, potentially up to 1000 dimensions. Vectorization is the process of turning words into numerical vectors. 

**A dense vector** is a vector where most of the entries are not zero. It is the opposite of a sparse vector such as one-hot encoding, which has many zero entries. This high-dimensional space is called the embedding space.

Words that have similar meanings or are used in similar contexts are assigned similar vectors, which means they are located close to each other in the embedding space. For example, “tea” and “coffee” are similar words that would be located close to each other, whereas “tea” and “sea” would be farther apart because they have dissimilar meanings and are not used together often, even though they have similar spelling.

While there are different methods of creating word embeddings in natural language processing, they all involve training on a large amount of text data called a corpus. The corpus can vary; Wikipedia and Google News are two common examples used for pre-trained embedding corpora.

The corpus can also be a custom embedding layer, which is specifically designed for the use case when other pre-trained corpora cannot supply sufficient data. During training, the model learns to associate each word with a unique vector based on the patterns of word usage in that data. These models can be used to transform words in any new text data into dense vectors.

### Summary:

Vector embeddings are a way to convert any type of data (most commonly sentences and words) to numbers (basically vectors) that are able to capture meaning and relationships.

The vectors are dense (meaning most data points are not zero) and high-dimensional (could be up to 1000 dimensions). The space in which the vectors are represented are the embedding space.

Words that are similar are closely represented within the embedding space. For example, “tea” and “coffee” are similar words that would be located close to each other, whereas “tea” and “sea” would be farther apart even though they have similar spelling.