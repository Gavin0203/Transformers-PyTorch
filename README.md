# Transformers-PyTorch

This repository contains a soft implementation of the paper "Attention Is All you need." or also called as Transformers.

The transformers architecture as seen below contains 3 important components:

1. Self-Attention Mechanism.
2. Encoder.
3. Decoder.

![alt text](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.analyticsvidhya.com%2Fblog%2F2019%2F06%2Funderstanding-transformers-nlp-state-of-the-art-models%2F&psig=AOvVaw1eYzr6fUSruXfTKoWKRhMe&ust=1664223983320000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCKCItM7jsPoCFQAAAAAdAAAAABAD)

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.analyticsvidhya.com%2Fblog%2F2019%2F06%2Funderstanding-transformers-nlp-state-of-the-art-models%2F&psig=AOvVaw1eYzr6fUSruXfTKoWKRhMe&ust=1664223983320000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCKCItM7jsPoCFQAAAAAdAAAAABAD" style=" width:700px ; height:500px ">

## Self-Attention Mechanism

In their paper, Attention Is All You Need, Vaswani et al. (2017) explain that the Transformer model, alternatively, relies solely on the use of self-attention, where the representation of a sequence (or sentence) is computed by relating different words in the same sequence. 

`Self-attention, sometimes called intra-attention is an attention mechanism relating different positions of a single sequence in order to compute a representation of the sequence.`
– Attention Is All You Need, 2017.

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fdata-science-blog.com%2Fblog%2F2021%2F04%2F07%2Fmulti-head-attention-mechanism%2F&psig=AOvVaw3mvoyTwfiGlXp8FaPkScMJ&ust=1664228438025000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCICp1KX0sPoCFQAAAAAdAAAAABAD" style=" width:700px ; height:500px ">


## Encoder

The encoder in the transformer consists of multiple encoder blocks. An input sentence goes through the encoder blocks, and the output of the last encoder block becomes the input features to the decoder. The decoder also consists of multiple decoder blocks. Each decoder block receives the features from the encoder.

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.researchgate.net%2Ffigure%2FThe-Transformer-encoder-structure_fig1_334288604&psig=AOvVaw2eKwosyXrKrrgnxUFQkrmT&ust=1664228594940000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCOD-6uT0sPoCFQAAAAAdAAAAABAJ" style=" width:700px ; height:500px ">

## Decoder

The decoder’s job is to generate text sequences. The decoder has a similar sub-layer as the encoder. it has two multi-headed attention layers, a pointwise feed-forward layer, and residual connections, and layer normalization after each sub-layer. These sub-layers behave similarly to the layers in the encoder but each multi-headed attention layer has a different job. The decoder is capped off with a linear layer that acts as a classifier, and a softmax to get the word probabilities.

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fdatascience.stackexchange.com%2Fquestions%2F96285%2Fstruggling-to-understand-implement-transformer-decoder&psig=AOvVaw2aC-9J0x06jNzT6fHH25w_&ust=1664229367902000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCJjvidb3sPoCFQAAAAAdAAAAABAI" style=" width:700px ; height:500px ">

## References.
1. https://jalammar.github.io/illustrated-transformer/
2. https://www.youtube.com/watch?v=U0s0f995w14