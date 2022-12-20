# Tuning-Convolutional-Neural-Networks

Note that model checking based on validation loss has been used to save the best model in the training process.
Metrics such as True Negatives or True positives have been used from time to time.

In steps 1 to 4 we try to find a good structure and in step 5 (which has several steps of its own), tuning of the parameters happen.

Step 1 : Trying random CNN models on our dataset to find a good base model using Keras


Step 2 : Using the best model from Step 1 and adding data augmentation, dropout layer. Then using VGG16 and Imagenet weights in fine tuning a model and trying to get better results. I only unfroze the last 4 layers of the conv base(VGG16) to finetune at the end.


Step 3 : Using ResNet50 instead of VGG16 in the fine tuning process.


Step 4 : The best model so far.


Step 5 : Tuning different settings of our best model
