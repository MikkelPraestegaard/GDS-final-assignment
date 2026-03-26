# GDS-final-assignment
Very cool project made by very cool students

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
\Data: 
Our data containing the small news sample and the entire LIAR dataset (train,val,test)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

Albert_predictions.csv: 
The predictions the Albert model gave on the labels of the FakeNews dataset.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

Albert.ipynb:
The pretrained Albert model is downloaded, and the code in the notebook is for fine-tuning it to our article classification task.
Running this notebook with a GPU is highly advised.

Albert.ipynb - Utilized packages:

sklearn.model_selection (train_test_split)
datasets (Dataset, load_dataset, Features, Value)
transformers (AlbertTokenizer, AlbertForSequenceClassification, Trainer, TrainingArguments, EarlyStoppingCallback, DataCollatorWithPadding)
sklearn.metrics (f1_score)
pandas
numpy
huggingface_hub (hf_hub_download)
torch

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

Code.ipynb:
This notebook contains our pipeline consisting of data preprocessing, exploratory data analysis, training, validation, testing and model evaluation. 
Running this notebook with a GPU is highly advised because we evaluate the Albert model, which can be time and RAM consuming.

Code.ipynb - Utilized packages:

matplotlib (+pyplot)
pandas
numpy
sklearn.model_selection (train_test_split)
regular expressions (re)
nltk.corpus (stopwords)
Stemmer
tqdm.notebook
sklearn.feature_extraction.text (CountVectorizer)
sklearn.linear_model (LogisticRegression)
sklearn.metrics (f1_score)
gc
collections (Counter)
sklearn.metrics (confusion_matrix)
transformers (AlbertTokenizer, AlbertForSequenceClassification, DataCollatorWithPadding)
torch