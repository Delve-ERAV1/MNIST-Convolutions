<h1 align="center"> 6 Iteration Analysis Report</h1>

# STEP-1

### Target
- Get the setup right
- Make sure everything is working
- Set the train loader and make a basic model(We can take care of parameters in the next steps)
- Train for 15 epochs

### Result
- Highest Train Accuracy - 99.91
- Highest Test Accuracy - 99.20
- No of parameters - 457k

### Analysis
- The model is overfitting since further training not all result in accuracy increase as the train accuracy has reached to max(99.91)
- We should change the model architecture and Normalize the input
### Plots for step-1
![download (1)](https://user-images.githubusercontent.com/62477860/120837482-5f4a6c80-c584-11eb-9745-a050e255ae39.png)

# STEP-2

### Target 
1. Change the model architecture

2. Try to decrease the parameters

### Result

1. Highest Train Accuracy -99.14

2. Highest test Accuracy - 98.89

3. No of Parameters - 20k

### Analysis

1. The graph shows that the loss is not fluctuating now it becomes constant after some point

2. The Model is not overfitting now. We can improve the model performance

### Plots for Step-2
![download (2)](https://user-images.githubusercontent.com/62477860/120837567-79844a80-c584-11eb-8e03-04e530ca8b04.png)


# STEP-3

### Target 

1. Apply batchnormalization 

2. Apply regularization(drop out)

3. Reduce the no of parameters

### Result

1. Highest Train Accuracy -99.33

2. Highest test Accuracy - 99.39

3. No of Parameters - 16k

### Analysis

1. The model works well enough

2. The Model is not overfitting now. We can still improve the model performance to aim for higher accuracy

3. Further training gives 99.40+ accuracy but we still need to modify our model

### Plots for Step-3
![download (3)](https://user-images.githubusercontent.com/62477860/120837625-8ef97480-c584-11eb-917f-5019eff626a6.png)

# STEP-4

### Target 
1. Try to decrease the model parameters

2. Change the model architecture 

3. Add Global Average pooling and add one more layer after that to increase the performance


### Result

1. Highest Train Accuracy -98.94

2. Highest test Accuracy - 99.21

3. No of Parameters - 11.5k

### Analysis

Reduced the parameters

1. The graph shows that the loss is is in decreasing state

2. The Model is some what not performing well now. We can improve the model performance more 

### Plots for Step-4
![step-4](https://user-images.githubusercontent.com/62477860/120837682-a173ae00-c584-11eb-8c3d-4963e41bd356.png)

# STEP-5

### Target
1. Set the architecture to reduce the parameters under 10k

2. Add maxpooling correctly


### Result

1. Highest Train Accuracy -99.19

2. Highest test Accuracy - 99.36

3. No of Parameters - 9k

### Analysis

1. The graph shows that the loss is decreasing and no high fluctuations

2. The Model is not overfitting now. It works fine

3. But we still can train the model to get higher accuracy

### Plots for Step-5
![step-5](https://user-images.githubusercontent.com/62477860/120837742-b6504180-c584-11eb-8993-a110551bc738.png)

# Step-6

### Target
1. Set the architecture to reduce the parameters under 10k.

2. Get Consitent Accuracy 99.4% / reduce fluctuations.
### Result
1. Highest Train Accuracy -98.19

2. Highest test Accuracy - 99.49

3. No of Parameters - 7.5k
### Analysis
1. Reduced the dropout to 0.04

2. The accuracy is consistent

3. Applied Step lr to reduce fluctuations and Image Augmentation Techniques

```
EPOCH: 7
Loss=0.034668635576963425 Batch_id=468 Accuracy=97.74: 100%|██████████| 469/469 [00:42<00:00, 10.93it/s]

Test set: Average loss: 0.0220, Accuracy: 9931/10000 (99.31%)

EPOCH: 8
Loss=0.06437068432569504 Batch_id=468 Accuracy=98.00: 100%|██████████| 469/469 [00:46<00:00, 10.01it/s]

Test set: Average loss: 0.0189, Accuracy: 9945/10000 (99.45%)

EPOCH: 9
Loss=0.13179419934749603 Batch_id=468 Accuracy=98.09: 100%|██████████| 469/469 [00:42<00:00, 10.93it/s]

Test set: Average loss: 0.0189, Accuracy: 9941/10000 (99.41%)

EPOCH: 10
Loss=0.04678237810730934 Batch_id=468 Accuracy=98.12: 100%|██████████| 469/469 [00:43<00:00, 10.85it/s]

Test set: Average loss: 0.0186, Accuracy: 9943/10000 (99.43%)

EPOCH: 11
Loss=0.0484786331653595 Batch_id=468 Accuracy=98.19: 100%|██████████| 469/469 [00:42<00:00, 11.08it/s]

Test set: Average loss: 0.0188, Accuracy: 9940/10000 (99.40%)

EPOCH: 12
Loss=0.033591706305742264 Batch_id=468 Accuracy=98.17: 100%|██████████| 469/469 [00:42<00:00, 11.12it/s]

Test set: Average loss: 0.0181, Accuracy: 9945/10000 (99.45%)

EPOCH: 13
Loss=0.06325388699769974 Batch_id=468 Accuracy=98.21: 100%|██████████| 469/469 [00:42<00:00, 11.10it/s]

Test set: Average loss: 0.0180, Accuracy: 9949/10000 (99.49%)

EPOCH: 14
Loss=0.0154658118262887 Batch_id=468 Accuracy=98.17: 100%|██████████| 469/469 [00:43<00:00, 10.90it/s]

Test set: Average loss: 0.0180, Accuracy: 9948/10000 (99.48%)
```

### Plots for Step-6
[![image.png](https://i.postimg.cc/WtRGgCNr/image.png)](https://postimg.cc/5Q3QMPFN)
