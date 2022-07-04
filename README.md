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

We implemented Finetuning, like methodology. Our first approach to improve the output of GPT-2 is to finetune it with additional training data, which
will make the model more specialized for poetry generation. To do this, we compiled a collection
of English and Spanish poetry. 
### Evaluation method:

For evaluation we implemented the loss function in train and test datasets.

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


