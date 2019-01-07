# Human Protein Atlas Image Classification

Classify subcellular protein patterns in human cells


> Please install [Open in Colab](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo) extension in Google Chrome in order to open a Github-hosted notebook in Google Colab with one-click.


## Background

### Description

<p><img align="right" src="https://storage.googleapis.com/kaggle-media/competitions/proteins/description_NACC_cropped_opt.png" width="20%"/></p>

In this competition, Kagglers will develop models capable of classifying mixed patterns of proteins in microscope images. [The Human Protein Atlas](https://www.proteinatlas.org/) will use these models to build a tool integrated with their smart-microscopy system to identify a protein's location(s) from a high-throughput image.

Proteins are "the doers" in the human cell, executing many functions that together enable life. Historically, classification of proteins has been limited to single patterns in one or a few cell types, but in order to fully understand the complexity of the human cell, models must classify mixed patterns across a range of different human cells.

Images visualizing proteins in cells are commonly used for biomedical research, and these cells could hold the key for the next breakthrough in medicine. However, thanks to advances in high-throughput microscopy, these images are generated at a far greater pace than what can be manually evaluated. Therefore, the need is greater than ever for automating biomedical image analysis to accelerate the understanding of human cells and disease.


> *[Nature Methods](Nature Methods) has indicated interest in considering a paper discussing the outcome and approaches of the challenge. The Human Protein Atlas team would like to invite top performing teams to join as co-authors in the writing of this paper.*
> 
> *Top performing teams will also be eligible to compete for the special prize. Additional information for both the special prize and co-authoring for Nature Methods will become available through the Discussion posts once the main competition is complete.*


### Acknowledgements

The Human Protein Atlas is a Sweden-based initiative aimed at mapping all human proteins in cells, tissues and organs. All the data in the knowledge resource is open access to allow anyone to pursue exploration of the human proteome. In a recent publication, the Human Protein Atlas team has demonstrated the promise of both citizen science and artificial intelligence approaches in describing the location of human proteins in images, however current results are yet to approach expert-level annotations ([Sullivan et al, Nature Biotechnology, Oct 2018](https://www.nature.com/articles/nbt.4225)).



## Data Description


### File descriptions

- **train.zip** - a folder containing the training images
- **train.csv** - maps the training `Image` to the appropriate whale `Id`. Whales that are not predicted to have a label identified in the training data should be labeled as `new_whale`.
- **test.zip** - a folder containing the test images to predict the whale `Id`
- **sample_submission.csv** - a sample submission file in the correct format

### Data fields

- `Id` - the base filename of the sample. As noted above all samples consist of four files - `blue`, `green`, `red`, and `yellow`.
- `Target` - in the training data, this represents the labels assigned to each sample.



## Q&A


- Mount Google Colab to your `Google Drive`

    ```python
    from google.colab import drive
    drive.mount('/content/drive/')
    
    cd drive/My\ Drive
    ```