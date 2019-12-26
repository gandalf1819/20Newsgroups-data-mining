# 20Newsgroups-data-mining

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

Using LIME and Spark MLlib, validate sentiment analysis using two classes - Atheism and Christianity with spark data pipeline and calculating F1-score, accuracy and class probabilities

## Installation

The lime package is on [PyPI](https://pypi.python.org/pypi/lime). Simply run:

```sh
pip install lime
```

Or clone the repository and run:

```sh
python setup.py install
```
## Screenshots

Below are some screenshots of lime explanations. These are generated in html, and can be easily produced and embedded in ipython notebooks. We also support visualizations using matplotlib, although they don't look as nice as these ones.

#### Two class case, text

Negative (blue) words indicate atheism, while positive (orange) words indicate christian. The way to interpret the weights by applying them to the prediction probabilities. For example, if we remove the words Host and NNTP from the document, we expect the classifier to predict atheism with probability 0.58 - 0.14 - 0.11 = 0.31.

![twoclass](https://github.com/marcotcr/lime/blob/master/doc/images/twoclass.png)

#### Multiclass case

![multiclass](https://github.com/marcotcr/lime/blob/master/doc/images/multiclass.png)

#### Tabular data

![tabular](https://github.com/marcotcr/lime/blob/master/doc/images/tabular.png)

#### Images (explaining prediction of 'Cat' in pros and cons)

<img src="https://github.com/marcotcr/lime/blob/master/doc/images/images.png" width=200 />

## Tutorials and API

For example usage for text classifiers, take a look at the following two tutorials (generated from ipython notebooks):

- [Basic usage, two class. We explain random forest classifiers.](https://marcotcr.github.io/lime/tutorials/Lime%20-%20basic%20usage%2C%20two%20class%20case.html)
- [Multiclass case](https://marcotcr.github.io/lime/tutorials/Lime%20-%20multiclass.html)

For classifiers that use numerical or categorical data, take a look at the following tutorial (this is newer, so please let me know if you find something wrong):

- [Tabular data](https://marcotcr.github.io/lime/tutorials/Tutorial%20-%20continuous%20and%20categorical%20features.html)
- [Tabular data with H2O models](https://marcotcr.github.io/lime/tutorials/Tutorial_H2O_continuous_and_cat.html)

For image classifiers:

- [Images - basic](https://marcotcr.github.io/lime/tutorials/Tutorial%20-%20images.html)
- [Images - Faces](https://github.com/marcotcr/lime/blob/master/doc/notebooks/Tutorial%20-%20Faces%20and%20GradBoost.ipynb)
- [Images with keras](https://github.com/marcotcr/lime/blob/master/doc/notebooks/Tutorial%20-%20Image%20Classification%20Keras.ipynb)
- [MNIST with random forests](https://github.com/marcotcr/lime/blob/master/doc/notebooks/Tutorial%20-%20MNIST%20and%20RF.ipynb)
- [Images with pytorch](https://github.com/marcotcr/lime/blob/master/doc/notebooks/Tutorial%20-%20images%20-%20Pytorch.ipynb)

For regression:
- [Simple regression](https://marcotcr.github.io/lime/tutorials/Using%2Blime%2Bfor%2Bregression.html)

Submodular Pick :
- [Submodular Pick](https://github.com/marcotcr/lime/tree/master/doc/notebooks/Submodular%20Pick%20examples.ipynb)

The raw (non-html) notebooks for these tutorials are available [here](https://github.com/marcotcr/lime/tree/master/doc/notebooks).

The api reference is available [here](https://lime-ml.readthedocs.io/en/latest/).

## Dataset

The dataset for this project is the 20 Newsgroups dataset which is a collection of approximately 20,000 newsgroup documents, partitioned (nearly) evenly across 20 different newsgroups.

http://qwone.com/~jason/20Newsgroups
