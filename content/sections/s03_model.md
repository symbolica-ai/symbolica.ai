---
title: "Symbolica Model"
weight: 3
improvecontrast: false
---

# The Symbolica Model

## Unsupervised, Online

Symbolica models are built using computational logic derived directly from the input data. Compiling a model requires no loss function, no back propagation, and no labels. The models compress and encode their own understanding of the input space, and can be trained to detect features in the data after compilation. This reversal of the training process makes it quicker and cheaper to build a model than has ever been possible before.

Training and inference are the same process, and the model is continually refining its own understanding of the input space as more data is provided. This means that the models can be deployed online, and will continue to improve as more data is provided.

## No Epochs? Epic.

Without relying on SGD, there is no need to train the same input data multiple times. Whereas neural networks require hundreds or thousands of epochs to converge, Symbolica models are compiled in a single pass. In practice we see Symbolica models converge using less than 1% of the data required for statistical methods.

## Hardware Accelerated

Symbolica models reduce to alternating linear and non-linear matrix operations, the same functions used for inference by traditional ML approaches. This means Symbolica models can take advantage of the last decade of hardware development into accelerating neural network inference. Since inference and training are the same process for Symbolica models, they are able to leverage that speedup for training as well.