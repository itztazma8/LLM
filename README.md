# Welcome to LLM 101!
The building blocks of LLM are important to understand LLM fully. So, many innate functionalities have been implemented from scratch with the goal of understanding these concepts. They are divided into sections as well. 
## Tokenizer & Embedding
A basic form of tokenizer has been made using a poetry dataset. Encoders and decoders can be found functioning in a class as well. 
## Attention Mechanism With Trainable Matrices
First, a simple context vector was made without trainable matrices. This is the ordinary version with all the necessary steps, such as attention matrix creation, context vector creation. In the next version, there are three matrices, namely- Query, Value & Key Vectors. Query & Key vectors are used to form an attention vector. Then it is scaled and normalized as well. Lastly, using the value matrix, the context vector is found.
## Causal Attention Mechanism
Another way to do this is by way of masking many of the values that we see in this process. The previous key, value, and query vectors are reused here. But later down the line, we first mask the values diagonally. Then, using the Dropout function, with a probability of 40%, we mask random values to finally get the context vector. The goal of this is to make sure the model works properly, as sometimes some values do not contribute in many deep learning scenarios.
