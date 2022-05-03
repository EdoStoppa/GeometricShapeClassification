# Geometric Shapes Classification
A Computer Vision project where a CNN learns ti recognize different geometric shapes in simple RGB pictures

## Dataset
The dataset is composed of 90000 images of geometric shapes: `Circle`, `Nonagon`, `Octagon`, `Heptagon`, `Hexagon`, `Pentagon`, `Square`, `Triangle`, and `Star`.
For each category, 10000 200x200 RGB pictures are present.

<div align="center">
  <img src="https://github.com/EdoStoppa/EdoStoppa/blob/main/imgs/GeometricShapeClassification/star.png?raw=true" alt="Star">
  <img src="https://github.com/EdoStoppa/EdoStoppa/blob/main/imgs/GeometricShapeClassification/pentagon.png?raw=true" alt="Pentagon">
  <img src="https://github.com/EdoStoppa/EdoStoppa/blob/main/imgs/GeometricShapeClassification/circle.png?raw=true" alt="Circle">
<div />
<div align="left"><div />
  
The dataset was split in the following way:
- 64% Training
- 20% Testing
- 16% Validation
  
During training the batch dimension was set to 32 (after some testing, this was the best value to lower the training time without losing any accuracy).
    
## Model
The idea is simple, but effective. I decided tu use 2 Convolutional layers and 2 Max-pooling layers (4x4). Then we have 3 fully connected layers
No dropout or batch normalizaion was needed, because in only 12 epochs the network reaches an accuracy of 85%.
<div align="center">
  <img src="https://github.com/EdoStoppa/EdoStoppa/blob/main/imgs/GeometricShapeClassification/nn.png?raw=true" alt="Neural Network">
  <img src="https://github.com/EdoStoppa/EdoStoppa/blob/main/imgs/GeometricShapeClassification/accuracy.jpg?raw=true" alt="Accuracy">
<div />
<div align="left"><div />
  
## More info
More information is written directly into the notebook, so if curious, please give a look at it.
