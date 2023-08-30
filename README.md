# African Style: Personalizing Stable Diffusion for Text-to-Image generation using Textual Inversion


### Bias in Text-to-Image models: Stable diffusion

![bias](https://github.com/opeajayi/18655-Project/assets/87567056/e2646966-53e9-40b0-8550-ab81679a3dae)

![bias2](https://github.com/opeajayi/18655-Project/assets/87567056/b2847976-765d-4e36-af01-1f1cbcc0575a)

 



### Abstracts
Artificial intelligence research in the area of computer vision teaches machines to comprehend and interpret visual data. In recent years, there has been significant development in text-to-image models which combine language and generative image models, to generate images based on textual prompts. In this project, we will be using Stable Diffusion (a text-to-image model) for two main tasks. First, we will generate detailed images conditioned on text descriptions using the model, and secondly, we will train the model to perform textual inversion using African contextual images such that when provided with a text prompt, the model can generate images in the style of the African images used to train the model. Focusing specifically on the second task, we present an approach to guide the creation of a text-conditioned image such that it models an African context. Using only 3-5 images representing African concepts, like an object or style, we learn to represent this concept through new “words” in the embedding space of a frozen text-to-image model. These “words” can be composed into natural language sentences, guiding personalized creation in an intuitive way.

![Final-African-Textual-Inversion Architecture](https://github.com/opeajayi/18655-Project/assets/87567056/532778cc-dec6-44c0-a706-ad246d2eb7ba)

### Description
This repo contains the official code , data and sample inversions for African style personalization of text-to-image  using textual inversion.

### Datasets
The pretrained model was trained on the LAION-5b dataset. The dataset contains 5.85 billion CLIP-filtered image-text pairs. It consists of 2.3 billion English language samples, 2.2 billion samples from 100+ other languages and 1 billion samples have texts that do not allow a certain language assignment (e.g. names). For the first task, we made use of the Stable Diffusion model pre-trained on this dataset to generate images based on textual prompts. 

For the textual inversion task of this project, we made use of self-curated African images with pixel size of 512 x 512 as training data to be supplied to the model. The images used were obtained from open-source high-quality websites to ensure that the images used are clear and of a resolution that does not reduce the performance of the model. 

Here are some generated samples: 
