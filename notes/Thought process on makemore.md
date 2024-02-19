---
share: true
---

It is a character-level generative DL model. The goal is to predict the next token, in this case, token equals to a character.

We first need to calculate the total number of vocabulary. This was done by go through the texts and do a set on every characters. Every character (token) will be assigned to a unique value to represent it.

We are not using one hot encoding, so we need to find out an embedding for each token. That would require us to have an embedding layer first to convert the token into a vector. The vector is usually one dimension, but with 32 (?) (i.e,  shape would be (1,32)?)

In order to predict the next token, we need certain inputs. We will use three tokens in the training texts, and the fourth token is the output. We will train based on this.

