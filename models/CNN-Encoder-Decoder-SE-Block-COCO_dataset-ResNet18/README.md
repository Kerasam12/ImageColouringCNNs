# CNN Encoder Decoder SE Block with COCO using pretrained ResNet18

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adriangar8/Artificial-Intelligence-degree_UAB/blob/master/CNN_Encoder_Decoder_SE_Block_COCO_dataset_ResNet18.ipynb)

In this computational notebook, we have implemented a convolutional autoencoder that incorporates a pretrained ResNet18 model for the encoder part. The purpose of using the pretrained ResNet18 is to leverage its learned features from the ImageNet dataset, allowing for fine-tuning and accelerated training. The decoder part of the autoencoder consists of a deconvolution architecture with four layers, which receives information from the pretrained ResNet18 model and incorporates a Squeeze-and-Excitation (SE) block. The SE block strategically integrates within the encoder-decoder modules to enhance the model's performance by emphasizing the most relevant filters for the color reconstruction task.

This design adaptation is specifically tailored to address the color reconstruction task, primarily focusing on our dataset that comprises various facial images. We have diligently utilized this dataset for both the training and testing processes, providing a comprehensive and relevant knowledge base for the model to learn from.

For readers seeking a deeper understanding and technical insights into Squeeze-and-Excitation Networks, we recommend referring to the scholarly work titled "Squeeze-and-Excitation Networks" by Hu et al., which was presented at the Computer Vision and Pattern Recognition (CVPR) conference in 2018.

During the training of this model, we utilized a subset of the COCO dataset for validation purposes, which consists of 5000 images. The use of this reduced dataset was done to ensure simplicity and reasonable training time without compromising the overall model performance.

- Dataset: https://gist.github.com/mkocabas/a6177fc00315403d31572e17700d7fd9
- Model: CNN Encoder Decoder SE Block and freee ResNet18 

# Results

<img width="368" alt="Screen Shot 2023-05-29 at 9 00 49 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/31da481c-9a35-4228-869b-34fc38b3ebc5">

<img width="369" alt="Screen Shot 2023-05-29 at 9 00 58 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/d1355c5a-fed4-451a-92e6-7955b7df1d49">

<img width="269" alt="Screen Shot 2023-05-29 at 8 59 48 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/a14647a6-f4e3-43d7-8f4a-c224186e1f1c">

<img width="269" alt="Screen Shot 2023-05-29 at 9 00 00 PM" src="https://github.com/DCC-UAB/dlnn-project_ia-group_03/assets/113826268/50e5c334-b872-4005-8939-4aa437f5f405">

*The results obtained with this model seem blurry, however on some of the images the silhouette can be seen. It can then be said that a training with a higher number of epoch would probably be helpful. Lastly it must be pointed out that as the pretrained model used 3 channels to train corresponding to the RGB color space the and as the COCO image dataset is a more complex one the computational capacity to train thi model would be much higher.*
