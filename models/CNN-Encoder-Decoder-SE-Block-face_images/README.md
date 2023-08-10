# CNN Encoder Decoder SE Block with face images

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adriangar8/Artificial-Intelligence-degree_UAB/blob/master/CNN_Encoder_Decoder_SE_Block_face_images.ipynb)

In the present computational notebook, we have executed the implementation of a convolutional autoencoder that incorporates a Squeeze-and-Excitation (SE) block nestled between the encoder and decoder modules. This strategic integration of the SE block is aimed at 

amplifying the model's performance through discerning and accentuating the most pertinent filters for the task of color reconstruction.

This design adaptation originates from a deliberate focus on the coloring reconstruction task, which is primarily rooted in our dataset that comprises of various facial images. The dataset has been meticulously utilized for both the training and testing processes, offering a comprehensive and relevant knowledge base for the model to learn from.

For more in-depth understanding and technical insights about Squeeze-and-Excitation Networks, readers are referred to the scholarly work by Hu et al., titled "Squeeze-and-Excitation Networks", presented at the Computer Vision and Pattern Recognition (CVPR) conference in 2018.

- Dataset: https://github.com/2014mchidamb/DeepColorization/tree/master/face_images
- Model: Convolutional Neural Network

Technical note: The color space used in this implementation is LAB (L for lightness and a and b for the color-opponent dimensions)

*It must be pointed out that in order to be able to execute the the code properly the dataset must be downloaded from the link provided above and ideally it must be ran in google collab as it is set to do it like that.*

# Results

![FaceColorizationAttention1](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/75599724-727d-4a65-b9c5-4770f345a494)

![FaceColorizationAttention2](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/608725d6-9912-4513-9753-d99096262187)

![FaceColorizationAttention3](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/26e4aba0-0b8e-474c-bd7b-ff9fcbfc7367)

![FaceColorizationAttention4](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/87bc89a5-64b3-4c11-9b82-133ee9e5e536)

![FaceColorizationAttention5](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/8855137c-9fa6-4d17-8851-f06b90b6d1d8)
