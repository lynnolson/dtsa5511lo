# dtsa5511lo
final project for DTSA5511


<!-- ABOUT THE PROJECT -->
## About the final project
This project focuses on extracting entities from discharge summaries, a clinical NER task, using pre-trained large language models (LLMs.)

It was done for CU Boulder's DTSA5511 Introduction to Deep Learning.

The LLMs used include
- BERT
- ClinicalBERT
- ClinicalLongformer


### Dependencies

The code was developed with Python 3.10.4 and the following libraries and versions:
- numpy==1.24.4
- pandas==2.0.3
- sklearn==1.3.0
- torch==2.0.1
- transformers==4.31.0
- seqeval
- wandb==0.15.9

You will need a [Weights and Biases](https://wandb.ai/site) account.

The full environment setting can be installed through:
```
conda env create -f conda-environment.yaml
conda activate msds
```

### Data

The datasets are from [n2c2](https://portal.dbmi.hms.harvard.edu/projects/n2c2-nlp/). In particular they are from the '2010 i2b2/VA Challenge on Concepts, Assertions, and Relations in Clinical Text' and the 'Evaluating temporal relations in clinical text: 2012 i2b2 Challenge' competitions.  You have to apply to get access to this data as it involves patient data.

Save the 2010 dataset to a directory in the same directory as this notebook named data/i2b2/2010/.  Likewise, save the 2012 dataset to a directory in the same directory as this notebook named data/i2b2/2012/.

Run the notebook i2b2_2010_iob.ipynb to get the i2b2 2010 in the format expected by the clinicalNER.ipynb notebook.  Likewise, run the notebook i2b2_2012_iob.ipynb to get the i2b2 2012 in the correct format.

### Usage

All code may be found and run in the notebook clinicalNER.ipynb.  The notebook assumes that the above datafile is found in the same directory in which the notebook is run.
