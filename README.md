# Personally Identifiable Information Processing

This is code for a multi-lingual Named Entity Recognition and PII processor used to remediate PII in web scale large language datasets for training large langauge models. This code is not meant to be used for general purpose PII remediation. 

## Organization of Repo

- The repo is a clone of the neuralcoref repo in order to more easily modify the base neuralcoref code and to take advantage of its great organization
- The code in the ontology folder is for building and tokenizing text for words in the ontology
- The code in the pii folder includes code to perform NER and coref resolution needed for pii processing
- The code in the masakhane-ner folder is code for training transfomrer based NER models (BERT, Roberta, etc.)
- The data folder contains the data needed by the other modules to operate
- The contrib folder will contain code from the community which will draw from the PII hackathon

## PII Hackathon
This repo is also home for reference implementation for the PII Hackathon, run by Ontocord, AISC, and BigScience

- The code under the directory ontology will be used for Module 1.
- The code under the directory pii will be used for Module 2.
- The code under the directory masakhane-ner will be used for Module 3.
- TODO: Module 4, We will provide a reference implementation for an ensemble semi-supervised learning training of a transformer model
 
## Requirements and Installation

- pip install spacy==2.1.8
- git clone  https://github.com/ontocord/pii_processing
- cd pii_processing/
- python setup.py install
- python -m nltk.downloader punkt stopwords  wordnet
- python -m spacy download en_core_web_lg

## Usage
TODO

## Credits

This code is based on original code by Ontocord, LLC (https://github.com/ontocord), Hugginface's Nueralcoref (https://github.com/huggingface/neuralcoref) and MasakhaNER (https://github.com/masakhane-io/masakhane-ner) which is in turn based on HF Transfromers (https://github.com/huggingface/transformers/) and Faker (https://github.com/joke2k/faker) and includes inspiration from Presidio (https://github.com/microsoft/presidio) . 

All code is released under Apache 2.0, except Neuralcoref which is under the MIT License.

Data is licensed as specified in the various data folders.


