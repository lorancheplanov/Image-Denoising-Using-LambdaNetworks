# Image-Denoising-Using-LambdaNetworks
In our work we dealt with the popular task of image denoising and tried to cope with it through adaptation of lambda layers. “Lambda layers” is a new approach of self-attention mechanism that bypasses the expensive memory usage requirements of attention maps and makes an efficient use of RAM. It was used as a main part in our model for accomplishing our goal and achieved success in terms of memory, PSNR and SSIM compared to more classical models that demand much more memory and epochs to train. 



Data:

The data we used to examine our model is the CIFAR-10. It consists of 32x32 color images in 10 different classes. There are a total of 60000 images in the dataset: 50000 for training and 10000 for test. In addition, in order to visualize our results with better resolution and for gaining another sight of results from a different “dataset”, a few images were downloaded from the web and resized in our model from their high resolution to 512x512. 


Architecture:

![image](https://user-images.githubusercontent.com/78099481/109872200-c4847e00-7c74-11eb-978f-44bc0ec44af1.png)


The comparable models:
1. DnCNN
2. Convolutional auto-encoder

# Results 
Table of parameters:

![image](https://user-images.githubusercontent.com/78099481/109872994-d3b7fb80-7c75-11eb-90b0-0a7ad6c443a0.png)




Relation between PSNR, models’ number of parameters and the encoders’ output channels of our model:

![image](https://user-images.githubusercontent.com/78099481/109872573-4674a700-7c75-11eb-8039-a700175908d8.png)




Convergence graph of our model:

![image](https://user-images.githubusercontent.com/78099481/109872711-7754dc00-7c75-11eb-9d36-d528f276599b.png)




Impact of different noise types the models performances (CIFAR10 dataset):

![image](https://user-images.githubusercontent.com/78099481/109872815-9bb0b880-7c75-11eb-8366-39d4cd264ed4.png)




Visualization of models performance. The images were resized from higher dimensions to 512x512 and a closer view was captured for enabling to distinguish the differences between them:

![image](https://user-images.githubusercontent.com/78099481/109872875-aec38880-7c75-11eb-96dc-f27466213d88.png)



