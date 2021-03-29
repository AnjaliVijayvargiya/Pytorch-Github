# Pytorch-Github

I have created a single repository here for the pytorch codes.
Here, is a list (is better to follow the series approach).
1. Pytorch Gradient:
2. Pytorch Linear Regression on simple generated data with linspace
3. Autoencoder implementation in linear way
4. Autoencoder implementation in Convoluted way


### Pytorch Gradient
This code is all about how we can solve an quadratic mathematical equation and compute its derivative using Pytorch. This can compute with Pytorch autograd package which provides differentiation function for a tensor object. A tensor object requires an attribute naming as .requires_grad attribute. By providing its value True, it can track all operations that are performed on a Tensor object. Then I have used .backward function for compute the gradients for the equation. By using .grad attribute we can see the gradient value.

Equation: y = 5*x^2+9*x+3
  dy/dx = 10*x+9
  
### Pytorch Linear Regression on simple generated data with linspace
