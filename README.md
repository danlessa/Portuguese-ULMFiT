# Portuguese-ULMFiT

The weights for the embedding layer of a Portuguese ULMFiT Model trained on Wikipedia and for using with fastai library.

## Description

The weights were trained on an 2019-08-07 dump of the Portuguese Wikipedia by using the procedures given on the n-wave's ulmfit-multilingual repository <https://github.com/n-waves/ulmfit-multilingual>, and by using an GCP Tesla K80. The perplexity is given as 11.65 (54.8% accuracy on an 2.456 cross-entropy validation loss)

For getting instructions as how to use the weights, I refer to Antti Karlsson's finnish pretrained model on <https://github.com/AnttiKarlsson/finnish_ulmfit>, as he has an Jupyter notebook which shows on practice as how to use it.

## Listing

* portuguese_itos.pkl contains the vocabulary mappings on the pickle format.
* portuguese_weights.pth contains the weights on pytorch format.

Parameters used on ulmfit-multilingual:

```

{"dataset_path": "data/wiki/pt-100", "base_lm_path": null, "backwards": false, "bidir": false, "qrnn": false, "max_vocab": 60000, "tokenizer": "f", "pretrained_model": null, "emb_sz": 400, "nh": 1150, "nl": 3, "clip": 0.12, "bptt": 70, "rnn_alpha": 2, "rnn_beta": 1} 

```
