# The code generates declensions of Armenian, Azerbaijani and Georgian Languages

## Introduction

**electra-ka** is an open-source model for the Georgian language. 

The model is available on [huggingface hub](https://huggingface.co/jnz/electra-ka)

The model is trained on 33GB of Georgian text collected from 4854621 pages in the commoncrawl archive.

The [fine-tuned model](https://huggingface.co/jnz/electra-ka-discrediting) is also available on the hub.

```python
from transformers import ElectraTokenizerFast
model = ElectraForSequenceClassification.from_pretrained("jnz/electra-ka-discrediting")
tokenizer = ElectraTokenizerFast.from_pretrained("jnz/electra-ka")

inputs = tokenizer("your text goes here...", return_tensors="pt")
predictions = model(**inputs)
```
