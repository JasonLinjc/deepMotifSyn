# DeepMotifSyn: a deep learning approach to synthesize heterodimeric DNA motifs
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/kundajelab/tfmodisco/blob/master/LICENSE)

## Introduction
DeepMotiSyn is a deep learning based prediction model for sgRNA on-target knockout
 efficacy and genome-wide off-target cleavage profile prediction. 
 
 This model is based on a carefully designed hybrid deep neural network for model training and prediction.

Current version focuses on conventional NGG-based sgRNA design for SpCas9 in human species, for it is
 widely used in related experiments.
 
 
## Requirement
* python == 3.6
* tensorflow == 1.3.0
* sonnet == 1.9

## Usage
1. Digitalize sgRNA using the following **sgRNA Coding Schema**. Epigenetics features can be found in [ENCODE](https://www.encodeproject.org/).
2. Load models from model directories (untar them first!) in `trained_models`. 
3. Perform prediction.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)