# CNN Encoder Decoder SE Block with COCO dataset

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adriangar8/Artificial-Intelligence-degree_UAB/blob/master/CNN_Encoder_Decoder_SE_Block_COCO_dataset.ipynb)

In the present computational notebook, we have executed the implementation of a convolutional autoencoder that incorporates a Squeeze-and-Excitation (SE) block nestled between the encoder and decoder modules. This strategic integration of the SE block is aimed at 

amplifying the model's performance through discerning and accentuating the most pertinent filters for the task of color reconstruction.

This design adaptation originates from a deliberate focus on the coloring reconstruction task, which is primarily rooted in our dataset that comprises of various facial images. The dataset has been meticulously utilized for both the training and testing processes, offering a comprehensive and relevant knowledge base for the model to learn from. 

The main imporvement we present in this notebook is that we separated the channels of LAB colorspace and using the L channel as input, so the network only have to reconstruct 2 channels, the A,B ones. This dramatically reduces the possible numbers that the model have to predict, acomplishing a much fast training and good performance. 

For more in-depth understanding and technical insights about Squeeze-and-Excitation Networks, readers are referred to the scholarly work by Hu et al., titled "Squeeze-and-Excitation Networks", presented at the Computer Vision and Pattern Recognition (CVPR) conference in 2018.

For the training of this model we use the COCO validation part, that has 5000 images. The use of this reduced dataset if for the seek of simplicity and reasonable training time.

- Dataset: https://gist.github.com/mkocabas/a6177fc00315403d31572e17700d7fd9
- Model: CNN Encoder Decoder SE Block

Technical note: The color space used in this implementation is LAB (L for lightness and a and b for the color-opponent dimensions)

# Results

![ImageColoring_color10](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/43663096-ba95-4b04-b6ca-7a4482272548)

![ImageColoring_gray10](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/0e63a56b-fac9-47fc-aa42-c113fe94f521)

![ImageColoring_color7](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/9fef3b07-0a46-46b9-8c1a-6c0562604402)

![ImageColoring_gray7](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/379e3a42-8b50-4812-a648-e14e655685c5)

![ImageColoring1](https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/9d737061-d16b-44a2-944c-450f23482c85)
