# DistilBERT-BERT-Transformer-Fine-Tuning
The first script fine-tunes the DistilBERT model on a spam message classification dataset. It includes the following steps:

    Data Preprocessing: The dataset, 'Spam messages.csv', is loaded and the 'Category' column is mapped to numeric values (0 for ham, 1 for spam). The data is split into training and test sets.

    Tokenization: The messages are tokenized using the DistilBERT tokenizer, with padding and truncation to handle sequences up to 512 tokens.

    Dataset Creation: A custom SpamDataset class is defined to convert the tokenized data into PyTorch Dataset objects for use in training.

    Model Setup: The DistilBERT model is initialized with 2 labels (for binary classification), and training arguments are set, such as the number of epochs, batch sizes, and warmup steps.

    Training: The model is fine-tuned using the Trainer class, with evaluation performed after training.

    Evaluation: After training, the model's performance is evaluated on the test set using accuracy and a detailed classification report.

BERT Transformer Fine-Tuning (IMDb Movie Reviews Classification)

The second script fine-tunes the BERT model for sentiment analysis on the IMDb movie reviews dataset. Key steps include:

    Data Loading: The IMDb dataset is loaded using the datasets library, and text and labels are extracted. The data is split into training and test sets.

    Tokenization: Reviews are tokenized using the BERT tokenizer with padding and truncation to handle sequences up to 512 tokens.

    Dataset Creation: The IMDbDataset class is used to convert tokenized inputs into PyTorch Dataset objects for the model.

    Model Setup: The BERT model is initialized for binary sequence classification (2 labels), and training arguments are specified, including settings for training, logging, evaluation, and saving model checkpoints.

    Training: The model is trained using the Trainer class, with evaluation performed at regular intervals.

    Evaluation: The trained model is evaluated on the test set, and performance is reported using accuracy and a classification report.

Both scripts demonstrate the application of transformer models (DistilBERT and BERT) for fine-tuning on text classification tasks, with a focus on efficient training and evaluation.
