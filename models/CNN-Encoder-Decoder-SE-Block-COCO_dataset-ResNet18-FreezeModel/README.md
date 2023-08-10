# CNN Encoder Decoder SE Block COCO_dataset ResNet18 FreezeModel

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adriangar8/Artificial-Intelligence-degree_UAB/blob/master/CNN_Encoder_Decoder_SE_Block_COCO_dataset_ResNet18_FreezeModel.ipynb)

In the current computational notebook, we have implemented a convolutional autoencoder. The encoder part of the autoencoder utilizes the pretrained ResNet18 model, which enables us to fine-tune the model and expedite training by leveraging the features learned during training with the ImageNet dataset. For the decoder part, we have designed a deconvolution architecture consisting of four layers. This decoder architecture receives information from the pretrained ResNet18 model and incorporates a Squeeze-and-Excitation (SE) block. However, the decoder part is trained from scratch.

The incorporation of the SE block between the encoder and decoder modules serves the purpose of enhancing the model's performance in color reconstruction. This strategic integration enables the model to discern and emphasize the most relevant filters for the task at hand.

Our design adaptation is primarily motivated by the focus on color reconstruction, which is rooted in our dataset consisting of diverse facial images. Throughout the training and testing processes, we have meticulously utilized this dataset to provide a comprehensive and relevant knowledge base for the model to learn from.

For readers seeking a deeper understanding and technical insights into Squeeze-and-Excitation Networks, we refer them to the scholarly work titled "Squeeze-and-Excitation Networks" by Hu et al., which was presented at the Computer Vision and Pattern Recognition (CVPR) conference in 2018.

In this model's training process, we have utilized a subset of the COCO dataset for validation, comprising 5000 images. This reduced dataset was chosen to strike a balance between simplicity and reasonable training time.

- Dataset: https://gist.github.com/mkocabas/a6177fc00315403d31572e17700d7fd9
- Model: CNN Encoder Decoder SE Block and freee ResNet18 

# Results

<img width="371" alt="Screen Shot 2023-05-29 at 9 52 57 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/9b032576-7cd9-4afc-9aa1-12a529c8ed56">

<img width="371" alt="Screen Shot 2023-05-29 at 9 53 06 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/180f1d76-7e4c-4a44-b2f8-1385bdfad784">

<img width="370" alt="Screen Shot 2023-05-29 at 9 53 16 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/96270b63-c620-4ab4-8632-02ca26cfc6c0">

<img width="369" alt="Screen Shot 2023-05-29 at 9 53 23 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/0e3c4dce-46a2-4ade-9165-04fa7a14acda">

<img width="371" alt="Screen Shot 2023-05-29 at 9 55 56 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/df29b00e-6d2d-4c8f-9f79-1e8caf0b2bd7">

<img width="369" alt="Screen Shot 2023-05-29 at 9 56 04 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/c2d843c6-c1ad-497b-9c4b-ce33c36406bb">


*The results obtained with this model seem blurry, however on some of the images the silhouette can be seen. It can then be said that a training with a higher number of epoch would probably be helpful. Lastly it must be pointed out that as the pretrained model used 3 channels to train corresponding to the RGB color space the and as the COCO image dataset is a more complex one the computational capacity to train thi model would be much higher.*
