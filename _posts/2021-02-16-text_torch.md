---
layout: post
title:  Text datasets in PyTorch
category: PyTorch 
description: How to use text as datasets in PyTorch
---

Most of the tutorials found online refer to the Field and BucketIterator classes. However, PyTorch gives a warning regarding deprecation. Not much is available on the internet in this regard. However, Ben Trevett has an excellent series of notebooks in this regard. The following example is a similar work showing how to load data from a text file and process it in a model

For the complete notebook, refer to this file [refer to this repo](https://github.com/mmg10/pytorch_text_new)

Here's the gist:  
* After reading and splitting the data, we build a tokenizer that also lowers and truncates the sentences  
* After tokenization, the data is preprocessed using the sequential_transforms and then a dataset is created using TextClassificationDataset  
* A collator pads the sequences to the maximum length.  
* DataLoader is created using the well-known `torch.utils.data.DataLoader`   
* The model is created and trained!  
* A confusion matrix is plotted for illustration  

Hope this helps! Feel free to comment and make suggestions...


