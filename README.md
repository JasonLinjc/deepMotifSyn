# DeepMotifSyn: a deep learning approach to synthesize heterodimeric DNA motifs
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/JasonLinjc/deepMotifSyn/LICENSE)

## Introduction
DeepMotiSyn is a deep-learning-based model to synthesize heterodimeric motifs from monomeric motif pairs. 
 
This model consists of heterodimeric motif generator and evaluator. The generator is a U-Net-based neural network that down-convolutes a monomeric motif pair and then up-convolute to generate a heterodimeric motif. A downstream machine learning model is used as the evaluator to compute for the predicted probability that a generated heterodimeric motif is the true one, based on the motif sequence features and DNA-binding family. Together, the generator and evaluator provide an integrated tool that enables users to conveniently synthesize heterodimeric motifs using any motif pair of interests.

<img src="images/deepMotifSyn.png" width="90%" height="90%" class="center" />
 
## Requirement
* python == 3.7
* pytorch == 1.7
* xgboost == 1.3.3
* MATLAB Engine API

Here is a tutoral how to install MATLAB Engine API (https://www.mathworks.com/help/matlab/matlab_external/install-the-matlab-engine-for-python.html)

## Example

Here is a [synthesis example notebook](https://colab.research.google.com/github/JasonLinjc/deepMotifSyn/blob/main/FLI1_FOXI1_synthesis_example.ipynb) which can be run on colab: 

<a href="https://colab.research.google.com/github/JasonLinjc/deepMotifSyn/blob/main/FLI1_FOXI1_synthesis_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
