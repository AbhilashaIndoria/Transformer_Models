Transformer models
This repository contains notebooks to explain and train decoder only models (GPT like model), Encoder (Baby BERT), and Encoder-decoder models, The notebooks also explain preprocessing of raw text to get it ready to be used for training various models.
The "Encoder baby BERT" repository, utilizes CSVs (train and test) to train a BERT model.
The training process here runs for 5 epochs and utilizes CUDA. For proper training number of epochs should be increased.
The Data_preparation_forBERT" directory includes 2 notebooks, one that pre-processes IMDB data and the other one that pre-processes AGNEWS data.
The notebooks include, tokenization, manual vocabulary building, Masking (for both Masked language Modeling and Next Sentence Prediction Task), after the data is preprocessed,
the data has been saved in CSV files.
The iteration to save in CSV files runs 100 times to save the compute time, the pre-processing of IMDB data takes 2-3 hours.
The CSVs can then be utilized to train the BERT model.
In the end of the notebook, pre trained BERT tokenizer has also been utilized to eliminate the need of building vocab manually from sractch.
