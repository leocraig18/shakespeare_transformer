# Drunk Shakespeare GPT

## Overview

Simple Transformer-based Bi-gram language model implementation using Pytorch. The model is designed to learn from and generate text inspired by the works of Shakespeare. It's a decoder-only model, focused on generating character-level syntax similar to its training input, making it suited for creative text generation tasks (but not much else).

## Key Features:

- Decoder-Only Model: Optimized for text generation, not for translation or QA tasks.
- Residual Connections: Enhances the flow of information and gradients through the network.
- Layer Normalization Preceding Attention and Feedforward: A design choice differing from some conventional Transformer models, where layer normalization follows these blocks.
- Dropout: Implemented for regularization to prevent overfitting.
- Adaptive to Compute Resources: Capable of running on GPU for faster processing, with a fallback on CPU if GPU is not available

## Hyper-parameters

The model's behavior can be fine-tuned through several hyper-parameters defined as global variables in model.py. These include settings for batch size, block size, number of iterations, learning rate, number of embedding dimensions, number of heads in multi-head attention, number of layers, and dropout rate.

## Installation
```bash
pip install torch
```
## Usage
```bash
python3 main.py
```



