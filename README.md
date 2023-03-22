# SSL-Cifar10-ContrastiveLearning
- Pytorch Implementation


For the original paper, please refer to the link https://arxiv.org/abs/2002.05709

This project is a replication of SimCLR model on Cifar10 dataset. Due to limitations of computational resources, I have used 10000 images to train the model (1000 images per class). I trained the model (ResNet-50) for 500 episodes. 

I fine-tuned pre-trained model with different proportions of labeled data. 

Note: Even the model is not fully trained, there is a visible development between different t-SNE graphs of Randomly Initialized Network - Network trained for 375 episodes - Network trained for 500 episodes.

<img width="929" alt="image" src="https://user-images.githubusercontent.com/87897577/226417973-770a5f38-20d8-48e6-9735-427b493701a4.png">


- Fine-tuning: best validation accuracies of  pre-trained model (375 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
|  1 %    |   48.44%  |
| 10 %    |   71.09%  |
| 30 %    |   74.53%  |
| 50 %    |   76.55%  |

- Fine-tuning: best validation accuracies of pre-trained model (500 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
|  1 %    |   50.07%  |
| 10 %    |   72.97%  |
| 30 %    |   76.32%  |
| 50 %    |   78.2%   |
