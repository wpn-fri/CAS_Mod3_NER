## Project for CAS NLP module 3 - Machine learning

### Content
The goal of this project is to train a neural network, explore the architecture and parameters and test their influence on model performance.
Specifically, we have trained two separate BiLSTM models for Named Entity Recognition (NER) using the relatively small LitBank dataset (literary texts, see https://github.com/dbamman/litbank).
The two models use different embeddings: randomly initialised vs. pre-trained FastText embeddings (300d).
Both use identical architecture (layers, hidden dimension) and training parameters (dropout, learning rate) to ensure comparison.

Three notebooks:
- data_analysis.ipynb: data loading and preprocessing
- litbank_ner_fasttext.ipynb: model initialisation, training and evaluation
- ner_newtext.ipynb: inference testing using custom texts

Expected outcome: Given the small size dataset, the overall performance of the models remains modest.
Nevertheless, the model using FastText embeddings is expected to perform slightly better since it can benefit from the semantic "knowledge" of the pretrained model.
