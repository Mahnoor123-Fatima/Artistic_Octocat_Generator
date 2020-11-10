# Artistic_Octocat_Generator

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1q45vqbWUjjUx8zEHa2g3j-womIV2Jx9r#scrollTo=s_c2IUXz5oxQ)

## Artistic_Octocat_Generator using Convolutional Neural Networks for artistic style transfer

<img align="right" img src="https://raw.githubusercontent.com/Mahnoor123-Fatima/Artistic_Octocat_Generator/main/4ljocm.webp" width="250px">

## Introduction:
This repository contains (TensorFlow and Keras) code. I use artistic style of AI to generate Octocat paintings.
Here, I have used python to take an image of octocat and turn it into the style of any artist of my choosing. Google released a similar production known as “Deep Dream” in 2015, and the internet took it was throbbing enthusiasm. They essentially trained a Convolutional Neural Net that classifies images and then used an optimization technique to enhance the patterns in the input image as opposed to its own weights based on what the network had learned.

## How it Works?
1. Install Dependencies
2. Need a content image
   
   here is my content image:<br>
   <img src="https://github.com/Mahnoor123-Fatima/Artistic_Octocat_Generator/blob/main/octocat_images/octocat_6.jpg" width = "250px">
   
3. Need a style image

   here is my style image:<br>
   <img src="https://github.com/Mahnoor123-Fatima/Artistic_Octocat_Generator/blob/main/style_images/style_image11.jpg">
   
4. Now I convert both these images so that they are in a suitable form for numerical processing. I will be using the VGG network moving forward. Keras has wrapped this model really well for me to use easily as i will moving forward. VGG16 is a 16 layer convolutional net, created by Visual Geometry Group at Oxford.

5. The idea here is that a CNN pre-trained for image classification on thousands of different images already knows how to encode information in a contained image.
6. This is essentially an optimization where we have some loss function that measures the error value that we will be attempting to minimize. My loss function in this case can be decomposed into two parts:
    
  - Content Loss
  - Style Loss
7. For this, I need to perform two transformations:
  - Subtract the mean RGB value 
  - Flip the ordering of the multi-dimensional array from RGB to BGR 
8. After all the process we have final Generated Artistic image.
   here is my generated image:<br>
   <img src="https://github.com/Mahnoor123-Fatima/Artistic_Octocat_Generator/blob/main/Generated_image8.PNG" width="250px">

## Setup
1. Install Python (2.7), pip on your machine. The instructions to do this depend on your operating system (Linux, macOS, Windows), but there are many tutorials on the internet that should help you get started.

2. Once you have the above setup, it is quite easy to setup the notebook in this repository. You just need to clone a copy of this repository:
````
git clone https://github.com/Mahnoor123-Fatima/Artistic_Octocat_Generator.git

````


## Enjoy!

--------------------------------------------------------------------------------------------------------


[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](#)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat&label=Contributions&colorA=red&colorB=black	)](#)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](#)
