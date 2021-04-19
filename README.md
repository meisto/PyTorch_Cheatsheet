# <p align="center">PyTorch Cheatsheet</p>
### <p align="center">High-level overview of some frequently used commands</p>

Always work in progress!

## 1. About this document.
This is a personal cheatsheet I use when I forget some commands. Feel free to use it as you like.  

*Note:* This document does not aim to be comprehensible. It only contains the API calls I often use or those of methods that are widely used in the literature. I aim to add links to the official pytorch website for further information.

## 2. Library


### Loss functions:
```python
torch.nn.L1Loss  # Mean absolute error
torch.nn.MSELoss # Mean squared error
torch.nn.NLLLoss # Negative log likelihood loss
torch.nn.CrossEntropyLoss # Cross-Entropy loss
torch.nn.KLDivLoss # Kullback-Leibler divergence
```
*[Documentation](https://pytorch.org/docs/stable/nn.html#loss-functions)*

### Optimizers:
```python
lr = 1e-3 # learning rate
params = model.parameters() # model parameters

torch.optim.SGD(pars, lr=lr)   # Stochastic Gradient Descent
torch.optim.Adadelta(params, lr=lr, rho=0.9, eps=1e-6, weight_decay=0)
torch.optim.Adagrad(params, lr=lr, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-9)
torch.optim.Adam(params, lr=lr, betas=(0.9, 0.999), eps=1e-08, weight_decay=0, amsgrad=False)
torch.optim.LBFGS(params, lr=lr, max_iter=20, max_eval=None, tolerance_grad=1e-07, tolerance_change=1e-09, history_size=100, line_search_fn=None)
torch.optim.RMSprop(params, lr=lr, alpha=0.99, eps=1e-08, weight_decay=0, momentum=0, centered=False)
torch.optim.Rprop(params, lr=lr, etas=(0.5, 1.2), step_sizes=(1e-06, 50))
```
*[Documentation](https://pytorch.org/docs/stable/optim.html)*
