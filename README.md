# Transformers-Create-your-own-poem

# Create your own poem with GPT-2


The objective of this project is generate poetry with a Tranformer model. Through a technical and literary analysis, we explore a
GPT-2 model trained on a dataset of Edgar Allan Poe and Spaninsh poetry and fine tuned to
output new poems. We explore the implications of uploading the “consciousnesses” of famous thinkers using deep learning models, and
conclude with a brief analysis of our model’s generated poetry.

##  Related Work 
A number an academic applications have explored the creative potential of deep learning models. 
A paper published in 2012 titled, “Full-FACE Poetry Generation” explores the early applications
of corpus-based poetry generation and claims to be the first paper to achieve poetry generation
that satisfies the four standards of the FACE descriptive model [1]. Another poetry generation paper that was particularly well-written came out in 2018 titled, “Deep-speare: A joint neural model of poetic language, meter and rhyme” [2]. In this paper,
researchers used a Project Gutenberg dataset of 3,355 Shakespearean sonnets to to output quatrains of poetry that followed specific rules of rhyme and meter. However, all of the above applications are based on LSTM recurrent neural networks and these are not very optimal when you have very long series. 

## About this repository

In this repository you will find everything you need to reproduce our work

* Eda: You will find the code with exploratory data analysis.
* models: You will find all the models made, one for spaninsh poetry and other for Edgar Allan Poe. 
* data: Source of data used


## Models and results

To select the model, for each cluster, we trained 4 different binary classification models: SVM, XGB, KNN, NB (each of a different nature). To guarantee the performance of each one we used K-fold in which we partition the data 10 times. In this way we obtain a list of scores from which we can obtain some basic statistics: standard deviation, mean, average; The metrics used for the evaluation in each Fold were: AUC, F1-Score and Acuraccy. To balance the data we used SMOTE-TOMEK which creates an artificial sample according to the nearest neighbors of each point.

The best performing model was Xgboost for both cases, a summary of the metrics obtained is shown below.

**Model 1:**


**Model 2:**



## Conclusions
 
 

## Prerequisites


* python3
* transformers-3.0.2


## References

[1] Colton, Simon, Jacob Goodwin, and Tony Veale. "Full-FACE Poetry Generation." ICCC.
2012.

[2] Lau, Jey Han, et al. "Deep-speare: A joint neural model of poetic language, meter and
rhyme." arXiv preprint arXiv:1807.03491 (2018).


