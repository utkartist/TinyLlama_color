# TinyLlama_color
This is a project made in collaboration with intel's Unnati program.

In this project, we are making advanced artificial intelligence (AI) tools accessible on everyday laptops by using a compact language model called TinyLlama which is the smallest of all llms and thus resource efficient and inferencing it with Intel® OpenVINO™. Our goal is to enable powerful AI capabilities without needing expensive hardware like high-end graphics cards. We are training TinyLlama with a detailed dataset of color descriptions so it can understand and generate rich information about different colors. Users simply type a color name or color code into their laptop, and TinyLlama processes this input to produce a detailed, easy-to-read description of the color, which is then displayed on the screen. This makes advanced AI technology more affordable and available to everyone.

![lamb](https://github.com/utkartist/TinyLlama_color/assets/156819805/4c448428-9d77-40a4-96d9-1b5e59268c87)


Tiny Colors Chat Project
This repository contains code for training and deploying a compact language model using TinyLlama-1.1B-Chat-v1.0. The model is trained to recognize and generate responses related to color descriptions. The project includes steps for data preparation, model training, and inference.

Table of Contents
Installation
Usage
Project Structure
Data Preparation
Model Training
Inference
Contributing
License
Installation
Install the required packages using pip. The main packages needed include accelerate, peft, bitsandbytes, transformers, trl, torch, and datasets.

Usage
1. Clone the Repository
Clone the repository to your local machine.

2. Login to Hugging Face
Login to your Hugging Face account to access models and datasets.

3. Prepare the Data
Load the dataset, reformat it into the ChatML format, and convert it into the required structure for training.

4. Load Model and Tokenizer
Load the pre-trained TinyLlama model and the tokenizer, applying specific configurations for quantization and device mapping.

5. Train the Model
Set up the training arguments and configurations, then use the SFTTrainer to fine-tune the model on the prepared dataset.

6. Inference
Use the trained model to perform inference on new inputs, including exporting the model to ONNX format and running predictions.

Project Structure
data_preparation.py: Script for preparing the dataset.
model_training.py: Script for training the model.
inference.py: Script for performing inference using the trained model.
requirements.txt: List of required packages.
Data Preparation
The data is sourced from the "burkelibbey/colors" dataset on Hugging Face. It includes descriptions and corresponding color names. The data is reformatted into a suitable structure for training the model.

Model Training
The model training process involves setting up the PEFT configuration, defining training arguments, and using the SFTTrainer to fine-tune the model. The model is trained to understand and generate responses related to color descriptions.

Inference
The inference process demonstrates how to use the trained model for generating predictions. It includes steps for exporting the model to ONNX format and using it for real-time inference.

Contributing
Contributions are welcome! Please fork the repository and create a new branch for your changes. Ensure that any images or data you contribute adhere to the licensing requirements.

License
This project is licensed under the MIT License. See the LICENSE file for details.

![Screenshot 2024-07-08 032714](https://github.com/utkartist/TinyLlama_color/assets/156819805/f33fb2c1-1381-422a-aff1-b97bb364554e)


