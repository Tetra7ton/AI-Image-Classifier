![Banner](./banneraiimg.jpg)

# AI Image Classifier

AI Image Classifier is a machine learning model that can effectively classify real and AI generated images.

# Table of Contents

- [AI Image Classifier](#ai-image-classifier)
- [Table of Contents](#table-of-contents)
- [Brief Overview](#brief-overview)
- [Demo](#demo)
- [Installation](#installation)
- [Data Sources](#data-sources)
- [Model](#model)

# Brief Overview
[(Back to top)](#table-of-contents)

This project involved building a machine learning model that can classify real and AI generated images. The first step was to create a dataset comprising AI-generated and real images. To accomplish this, `pygoogle_image` was used, with which images from Google were downloaded. Apart from Google Images, two more datasets were used.

- CIFAKE: Real and AI-Generated Synthetic Images 
- Ai Generated Images | Images Created using Ai from Kaggle

These images were preprocessed and features were extracted. Then, a Convulutional Nueral Network based Classifier model was constructed and trained on the dataset containing around 1,00,000 images.

# Demo
[(Back to top)](#table-of-contents)

Here is a short demo of the deployed web application.

https://github.com/SanKolisetty/AI-Image-Classifier/assets/95172001/0ebe3ffb-4afe-4a7b-96d3-80ce5e7ce99f

# Installation
[(Back to top)](#table-of-contents)

Open Git Bash and change the directory to the location where the repository is to be cloned. Then, type the following commands.

```shell
  git init
```
```shell
  git clone https://github.com/SanKolisetty/AI-Image-Classifier.git
```
Now, install the requirements given below.

- Python3 
- TensorFlow 
- NumPy
- Streamlit
- Keras
- Pillow

To access or use the application, open a terminal in the cloned repository folder and run the following command.

```shell
  streamlit run deploy.py
```
Finally, browse the link provided in your browser.

# Data Sources
[(Back to top)](#table-of-contents)

The dataset comprised of Real and AI Generated Images. Images were collected from Google using the python library `pygoogle_image`. Every single image was verified to avoid issues such as incorrect and ambigous images. Two other datsets were also used.

- CIFAKE: Real and AI-Generated Synthetic Images ( [Link](https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images) )
- Ai Generated Images | Images Created using AI ( [Link](https://www.kaggle.com/datasets/anasmahmood000/ai-generated-images) )

Combing the three datasets, we have:

- Train Set: 101031
- Test Set: 20000

# Model

[(Back to top)](#table-of-contents)

The CNN model was built similar to `VGG16` and was trained on the train dataset. The following image show the model architecture.

![modelarchitecture](https://github.com/SanKolisetty/AI-Image-Classifier/assets/95172001/46b84444-8501-47ad-a0bb-9a778d2b1047)
