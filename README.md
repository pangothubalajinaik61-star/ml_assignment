# Understanding Residual Connections: Why Skip Connections Enable Deep Neural Networks to Train Effectively

## Overview
This project investigates why deeper neural networks can be difficult to train and how residual connections (ResNet) improve optimization.

The study focuses on understanding:
- gradient flow
- training dynamics
- the distinction between optimization and generalization

using controlled experiments on the Fashion-MNIST dataset.

---

## Objectives
- Explain why deep networks suffer from vanishing gradients and the degradation problem  
- Demonstrate how residual connections improve optimization  
- Compare shallow, deep plain, and deep residual neural networks  
- Analyze loss curves, gradient behaviour, and validation performance  

---

## Experiment Summary

Three models were implemented:

- ShallowCNN – baseline model  
- DeepPlainCNN – deeper network without skip connections  
- DeepResidualCNN – network with residual blocks  

### Key Findings
- Residual networks achieve the lowest training loss  
- Residual networks reach the highest peak validation accuracy  
- Deep plain networks show more stable final generalization  
- Residual connections improve optimization but do not inherently prevent overfitting  

---

## Results

| Model              | Parameters | Final Train Loss | Final Val Acc | Best Val Acc |
|------------------|-----------:|-----------------:|--------------:|-------------:|
| ShallowCNN       |   421,642  | 0.1197           | 0.9144        | 0.9206       |
| DeepPlainCNN     | 1,090,666  | 0.0941           | 0.9213        | 0.9251       |
| DeepResidualCNN  |   606,346  | 0.0626           | 0.9124        | 0.9287       |


## Installation


cd residual-connections-tutorial  

pip install -r requirements.txt  

---

## Usage

jupyter notebook  

Open:  
24162819_code.ipynb  

Run all cells to reproduce the results and figures.

---

## Requirements

- Python 3.x  
- PyTorch  
- torchvision  
- numpy  
- matplotlib  
- pandas  

---

## Accessibility

This project incorporates accessibility considerations:
- Figures include descriptive captions  
- Colour schemes are chosen to be readable and distinguishable  
- Content is structured with clear headings  
- Results are presented in readable tabular format  

---

## References

- He, K., Zhang, X., Ren, S., and Sun, J. (2016). Deep Residual Learning for Image Recognition  
- Glorot, X., and Bengio, Y. (2010). Understanding the difficulty of training deep feedforward neural networks  
- Goodfellow, I., Bengio, Y., and Courville, A. (2016). Deep Learning  

---

## License

This project is licensed under the MIT License.

---
