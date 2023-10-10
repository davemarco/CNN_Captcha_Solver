# CNN Captcha Solver
CAPTCHA solver powered by a custom convolutional neural network (CNN). 

# Model
The CNN consists of three convolutional layers and three pooling layers. The output is flattened, passed into a 512 neuron hidden layer, and finally connected to five output layers with 10 neurons each to obtain class probabilities. In total, the model has 264,674 trainable parameters. The layers were connected rectified linear unit activation function (ReLU) and the multi-class cross-entropy loss function was used. The network yielded best accuracy when learning rate was 0.01, batch size was 32, and the number of epochs was 10. 

![CNN_page-0001](https://github.com/davemarco/CNN_Captcha_Solver/assets/83603688/2ffbe1db-bd0d-4c15-afd1-21067c1f6779)

# Dataset
The dataset consists of 60,480 text-based CAPTCHAs generated using a [CAPTCHA library](https://pypi.org/project/captcha/). Each CAPTCHA had 5 numerical digits. The digits were distorted with random font size changes, rotations, translations, lines/curves and dots. The training/validation/test split was 70%/20%/10%.

![captcha1](https://github.com/davemarco/CNN_Captcha_Solver/assets/83603688/36c6ad51-cc07-4845-b69a-678364af9935)

# Results
Accuracy on the test set for the whole CAPTCHA was 82%. Accuracy for individial digits was 94%. 

# Demo on simple CAPTCHA
https://github.com/davemarco/CNN_Captcha_Solver/assets/83603688/952e3952-aaa8-47eb-8e18-a76c864f3be7








