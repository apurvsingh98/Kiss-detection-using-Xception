# Kiss-detection-using-Xception
This repository contains a basic implementation Xception used for detecting Kiss in an image.

    *It uses transefer learning by using the pretrained Keras's Xception treained on imagenet dataset.
The repository contains two ipynb notebooks explaining each steps for training your own model and then testing it.

Personal opinions on training the model

        *Run the model notebook preferebly on a gpu (I use colab for my experimentation).
        *Different hyperparameters can be used and tweaked for achieving the best accuracy.
        *I have used Adam optimizer with an intitial learning rate of 0.001 and later reduced it as the accuracy hit the plateau.
        *Different regularization techniques can be used, I have used Dropouts.
        *Different layers of the Xception model can be unfreezed for training depending on the available computational power. 
        *Last few dense layers can be also tweaked for a better result.
 
The repository also contains code for 

        *Resizing the images using OpenCV 
        *Removing corrupted images, which would get automatically deleted once run over a directory containing images

