# <p align="center">PyTorch Cheatsheet</p>
### <p align="center">High-level overview of some frequently used commands</p>

WIP!

## 1. About this document.
This is a personal cheatsheet I use when I forget some commands. Feel free to use it as you like.

## 2. Library


**Loss functions:**
```python
torch.nn.L1Loss  # Mean absolute error
torch.nn.MSELoss # Mean squared error
torch.nn.NLLLoss # Negative log likelihood loss
torch.nn.CrossEntropyLoss # Cross-Entropy loss
torch.nn.KLDivLoss # Kullback-Leibler divergence
```

**Optimizers:**
```python
learning_rate = 1e-3
torch.optim.SGD(model.parameters(), lr=learning_rate)   # Stochastic Gradient Descent
```
