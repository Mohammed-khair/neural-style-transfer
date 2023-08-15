# Neural Style Transfer Using TensorFlow

This repository contains a Jupyter Notebook that demonstrates Neural Style Transfer (NST) using TensorFlow. NST is a fascinating technique that combines the content of one image with the style of another to create visually appealing artworks.

## Acknowledgments

The code in this repository is based on a course project and assignments from the [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) on Coursera. 
The course materials provide valuable insights into the concepts and techniques underlying Neural Style Transfer.

## Table of Contents

- [Overview](#overview)
- [Content Cost](#content-cost)
- [Style Cost](#style-cost)
- [Total Cost](#total-cost)
- [Usage](#usage)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Overview

The provided Jupyter Notebook showcases the process of applying Neural Style Transfer to create a new image that merges the content of a chosen image with the artistic style of another. The NST process involves defining and optimizing two key components: the content cost and the style cost. These costs are combined to compute the total cost, which guides the optimization process towards generating the final stylized image.

## Content Cost

In the notebook, the concept of content cost is introduced. The content cost measures the difference between the activations of a content image and a generated image in a chosen hidden layer of a pre-trained neural network (VGG19 in this case). By minimizing this cost, the generated image gradually aligns its content with that of the content image while still preserving its unique style.

## Style Cost

The notebook delves into the notion of style cost. The style cost quantifies how closely the texture and patterns of the generated image match those of a style image. It's calculated using Gram matrices, which capture the correlations between different features in an image. By minimizing the style cost, the generated image gradually adopts the artistic style of the style image while retaining its original content.

## Total Cost

The notebook brings together the content cost and style cost to compute the total cost. The total cost is a weighted combination of the content cost and style cost, with adjustable hyperparameters alpha and beta. This total cost is the driving force behind the optimization process that shapes the generated image, aligning its content and style as desired.

## Usage

1. Clone this repository to your local machine.
2. Open the Jupyter Notebook `neural_style_transfer.ipynb`.
3. Run each cell in sequence to observe the NST process step by step.
4. Experiment with different content and style images, hyperparameters, and optimization iterations to create unique stylized images.
5. The generated images will be saved in the `output/` directory.



