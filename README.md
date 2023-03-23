# SSL-Cifar10-ContrastiveLearning
- PyTorch Implementation
- Self-Supervised Contrastive Learning

For the original paper, please refer to the link https://arxiv.org/abs/2002.05709

This project is a replication of SimCLR model on Cifar10 dataset. Due to limitations of computational resources, I have used 10000 images for pre-training (1000 images per class). I trained a model (ResNet-50) with a projection head for 500 episodes.


- Even the model is not fully trained, there is a remarkable development between different t-SNE graphs of                                    
  Randomly Initialized Network  - Network trained for 375 episodes -  Network trained for 500 episodes.

<img width="929" alt="image" src="https://user-images.githubusercontent.com/87897577/226417973-770a5f38-20d8-48e6-9735-427b493701a4.png">

- Fine-tuned pre-trained base encoder with varying percentages of labeled data for 30 episodes. --> 1%-10%-30%-50%

- Fine-tuning: best validation accuracies of  pre-trained model (375 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
|  1 %    |   47.30%  |         
| 10 %    |   71.33%  | 
| 30 %    |   74.75%  |
| 50 %    |   76.42%  |

- Fine-tuning: best validation accuracies of pre-trained model (500 episodes)

| % Label | Accuracy  | 
|  :---:  |   :---:   |
|  1 %    |   50.21%  |
| 10 %    |   72.68%  |
| 30 %    |   76.82%  |
| 50 %    |   78.06%  |

<img width="1031" alt="image" src="https://user-images.githubusercontent.com/87897577/227078015-f0a05e94-ca20-447b-9af6-f473bb8e0760.png">


