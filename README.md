# DeepMotifSyn: a deep learning approach to synthesize heterodimeric DNA motifs
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/JasonLinjc/deepMotifSyn/LICENSE)

## Introduction
DeepMotiSyn is a deep-learning-based model to synthesize heterodimeric motifs from monomeric motif pairs. 
 
This model consists of heterodimeric motif generator and evaluator. The generator is a U-Net-based neural network that down-convolutes a monomeric motif pair and then up-convolute to generate a heterodimeric motif. A downstream machine learning model is used as the evaluator to compute for the predicted probability that a generated heterodimeric motif is the true one, based on the motif sequence features and DNA-binding family. Together, the generator and evaluator provide an integrated tool that enables users to conveniently synthesize heterodimeric motifs using any motif pair of interests.
 <img src="images/deepMotifSyn.png"/>
 


## Requirement
* python == 3.6
* tensorflow == 1.3.0
* sonnet == 1.9

## Usage
1. Digitalize sgRNA using the following **sgRNA Coding Schema**. Epigenetics features can be found in [ENCODE](https://www.encodeproject.org/).
2. Load models from model directories (untar them first!) in `trained_models`. 
3. Perform prediction.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)
