This repo is adapted from course in deeplearning.ai by Josh Starmer

In this tutorial, we will code Masked Self-Attention in PyTorch. Attention is an essential component of neural network Transformers, which are driving the current excitement in Large Language Models and AI. Specifically, a Decoder-Only Transformer, illustrated below, is the foundation for the popular model ChatGPT.

<img width="1920" height="1080" alt="dec_transformer" src="https://github.com/user-attachments/assets/ab7c57ff-df55-49d0-bdca-04fda116d719" />


At the heart of ChatGPT is Masked Self-Attention, which allows it to establish relationships among the words, characters and symbols while also making it relatively easy to train the model to predict what should come next. For example, in the illustration below, where the word it could potentially refer to either pizza or oven, Masked Self-Attention could help a Transformer establish the correctly relationship between the word it and pizza as well as help efficiently train it to predict the words that came after, tasted good.

<img width="1920" height="540" alt="masked_self_attention_1" src="https://github.com/user-attachments/assets/c341995d-97ec-435d-9cd9-3d596edcee22" />



The the masked self-attention class allows the transformer to establish relationships among words and tokens and be efficiently trained to predict what comes next.

We'll then use the class that we created, MaskedSelfAttention, to calculate masked self-attention values for some sample data.
 
Lastly, we'll validate the calculations made by the MaskedSelfAttention class..
