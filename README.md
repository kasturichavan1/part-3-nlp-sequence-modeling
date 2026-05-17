# NLP Sequence Modeling - Customer Support Text Classification

## Task 1: Dataset Understanding

The dataset contains customer support messages along with sentiment labels.

### Dataset Analysis
- Number of records: Dataset loaded using pandas
- Target labels/classes: sentiment_label
- Text column: customer_message

### Sample Records
The dataset contains customer messages representing different customer sentiments.

### Average Text Length
The average text length was calculated using the length of customer messages.

### Class Distribution
The distribution of sentiment labels was analyzed and visualized using a bar graph.

---

## Task 2: Text Preprocessing

The following preprocessing techniques were applied to the text data:

- Lowercasing text
- Removing special characters and unnecessary symbols
- Tokenization
- Removing stopwords
- Converting text into padded sequences

These preprocessing steps help clean and standardize the text before model training.

---

## Task 3: Text Vectorization

Text data was converted into numerical vectors using:

- TF-IDF Vectorization
- Tokenizer-based sequences

### Why text must be converted into vectors

Machine learning models cannot directly understand raw text.  
Text must be converted into numerical representations so that patterns and relationships can be learned mathematically by the model.

---

## Task 4: Baseline Model

A Logistic Regression model was built using TF-IDF features.

### Evaluation Metrics
- Accuracy Score
- Classification Report

The model was trained and evaluated on customer sentiment classification.

---

## Task 5: Sequence Model Architecture

An LSTM-based sequence model was designed for text classification.

### Input Sequence
Customer messages were converted into padded numerical sequences.

### Embedding Layer
The embedding layer converts words into dense vector representations.

### Recurrent Layer
The LSTM layer learns sequential and contextual information from the text.

### Output Layer
A dense softmax layer predicts the sentiment class probabilities.

### Loss Function
Sparse categorical crossentropy

### Evaluation Metric
Accuracy

---

## Task 6: Attention and Transformer Reflection

### Why do RNNs struggle with long-term dependencies?

RNNs struggle to remember earlier information in long sequences because important information gradually fades during training.

### How do LSTMs help with memory?

LSTMs use memory cells and gates to remember important information for longer periods.

### What does attention solve in sequence-to-sequence tasks?

Attention helps the model focus on the most relevant words in the input sequence during prediction.

### Why are transformers important in modern NLP and Generative AI?

Transformers process text efficiently using self-attention mechanisms and are the foundation of modern AI models such as GPT and BERT.
