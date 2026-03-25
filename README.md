PROBLEM 1: LEARNING WORD EMBEDDINGS FROM IIT JODHPUR DATA
Objective

The objective of this problem is to train Word2Vec models on textual data collected from IIT Jodhpur sources and analyze the semantic relationships captured by the learned embeddings.

Dataset

The dataset consists of textual content collected from multiple IIT Jodhpur sources, including:

Official website pages (departments, academic programs, research pages)
Academic regulation documents
Faculty profiles and course-related information

Only English text was considered, and irrelevant or non-textual content was removed.

Preprocessing

The collected data was preprocessed using the following steps:

Removal of boilerplate content such as headers, menus, and navigation text
Conversion of text to lowercase
Removal of URLs, numbers, and special characters
Tokenization into words
Filtering of noise and non-informative words
Construction of clean sentences for training
Dataset Statistics
Total number of documents (sentences): [fill value]
Total number of tokens: 61382
Vocabulary size: [fill value]

Top frequent words include engineering, research, students, mtech, phd, and academic.

Models Implemented

Two Word2Vec models were implemented from scratch:

Continuous Bag of Words (CBOW)
Skip-Gram with Negative Sampling
Experiments

The models were trained with different configurations:

Embedding dimensions: 50, 100
Context window sizes: 2, 4
Negative samples (Skip-Gram): 2, 5
Results
CBOW produces smoother embeddings but is less precise
Skip-Gram captures better semantic relationships
Higher embedding dimensions improve performance
Smaller window sizes capture stronger local relationships
Increasing negative samples improves Skip-Gram performance
Semantic Analysis

Nearest neighbor analysis shows meaningful relationships such as:

student → teacher, professor
research → phd, academic

Analogy tasks demonstrate:

UG : BTech :: PG : MTech
student : teacher :: research : professor
Visualization

Word embeddings were visualized using PCA and t-SNE:

Words cluster based on semantic similarity
Skip-Gram produces more distinct clusters than CBOW
Conclusion

The trained embeddings successfully capture semantic relationships in academic data. Skip-Gram with negative sampling performs better than CBOW in most cases.




PROBLEM 2: [REPLACE WITH YOUR ACTUAL TITLE]
Objective

The objective of this problem is to design and implement sequence models such as RNN, BiLSTM, and Attention-based RNN, and compare their performance on sequence modeling tasks.

Models Implemented

The following models were implemented:

Recurrent Neural Network (RNN)
Bidirectional LSTM (BiLSTM)
Attention-based RNN
Methodology
Input text sequences were preprocessed and tokenized
Models were trained to learn sequential dependencies
Performance was evaluated using both quantitative and qualitative metrics
Results and Comparison
RNN captures only short-term dependencies and performs the worst
BiLSTM improves performance by using both past and future context
Attention-based RNN performs best by focusing on important words
Observations
Attention improves context understanding significantly
BiLSTM performs better than simple RNN
Attention-based models generate more meaningful and coherent outputs
Conclusion

Among the three models, Attention-based RNN performs best, followed by BiLSTM and RNN. The attention mechanism enhances performance by focusing on relevant parts of the input sequence.
