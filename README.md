# DL-Midterm-Project
Deep Learning Course Midterm Project

This mini-project focuses on the refinement of the Residual Network (ResNet) architecture for image classification task using the CIFAR-10 dataset, with the constraint of limiting the model to no more than 5 million parameters.

Throughout this project, we explored effects of different hyperparameters on the model’s performance. This includes adjustments to model architecture like number of channels, filter sizes, kernel sizes within skip connections and pool sizes. This iterative process allows for focusing on achieving superior accuracy while operating within the number of parameters limit. We also explored configurations for batch sizes, number of epochs, learning rate scheduling, and initialization methods. Furthermore, we explored various optimization techniques, such as SGD and ADAM, alongside the exploration of different data augmentation strategies and regularization methods.

<h2> &nbsp;Model Architecture</h2>

In our ultimate model, we used a Wide ResNet architecture of decreased depth (less layers) but increased width (number of filters) in the layers to achieve higher accuracy and reduce overfitting. Specifically, we use a ResNet containing 4 residual layers with [2, 3, 4, 3] residual blocks, respectively. The layers have increasing width going from [16, 16*4, 32*4, 64*4] filters. This is an overview of our model architecture:

<h2> &nbsp;Results</h2>
With our best model, we achieve a 93.7\% accuracy on the testing batch and a 82.5\% on the customized dataset after training for 100 epochs. 
The following figures depict the changes of the accuracy and the loss of our model over the entire training process:

Train versus validation accuracy over 100 epochs:

Train versus validation loss over 100 epochs:
