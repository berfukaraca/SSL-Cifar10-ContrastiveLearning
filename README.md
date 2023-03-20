# SSL-Cifar10-ContrastiveLearning_pytorch

This project is a replication of SimCLR model on Cifar10 dataset. Due to limitations of computational resources, I have used 10000 images to train the model (1000 images per class). I trained the model for 500 episodes. 

Note: Even the model is not fully trained, there is a visible development between different t-SNE graphs of Randomly Initialized Network - Network trained for 375 episodes - Network trained for 500 episodes.

<img width="929" alt="image" src="https://user-images.githubusercontent.com/87897577/226417973-770a5f38-20d8-48e6-9735-427b493701a4.png">


- Fine-tuning: best validation accuracies of  pre-trained model (375 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
| 10 %    |   71.09%  |

- Fine-tuning: best validation accuracies of pre-trained model (500 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
| 10 %    |   72.97%  |
| 30 %    |   76.32%  |
| 50 %    |   78.2%   |
