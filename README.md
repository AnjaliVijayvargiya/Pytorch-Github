# Pytorch-Github

I have created a single repository here for the pytorch codes.
Here, is a list (is better to follow the series approach).
1. Pytorch Gradient:
2. Pytorch Linear Regression on simple generated data with linspace
3. Autoencoder implementation in Linear way
4. Autoencoder implementation in Convoluted way


### Pytorch Gradient
This code is all about how we can solve an quadratic mathematical equation and compute its derivative using Pytorch. This can compute with Pytorch autograd package which provides differentiation function for a tensor object. A tensor object requires an attribute naming as .requires_grad attribute. By providing its value True, it can track all operations that are performed on a Tensor object. Then I have used .backward function for compute the gradients for the equation. By using .grad attribute we can see the gradient value.

Equation: y = 5*x^2+9*x+3

dy/dx = 10*x+9
  
### Pytorch Linear Regression on simple generated data with linspace
In this code, I have tried to develop a regression model to get the best-fit line for the equation of y = 4*x+4.

Steps:
1. Attaching Libraries
2. Create Linearly spaced array. Add noise and Calculate y. for making the staright line data slightly disturbed 
3. See the variation in data by matplotlib
4. Prepare a Regression Model with random weight and bias, In our case size of weight and bias are 1.
5. Save seed value for same result; Initial values for weight and bias.
6. Refer 2 coordinates for estimation of best fit line. that's why consider the min and max points.
7. Calculate y on 2 coordinates with inital values of weight and bias.
8. At the first epoch, the status of best fit line
9. Calculate MSE loss
10. Apply Stochastic Gradient Descent
11. Running Model for 50 epochs; Showing Epoch value, Loss value, updated Weight and bias value at each epoch. 
12. plot between Loss and Epochs
13. Current values for weight and bias after 50 epochs
14. At the last epoch, the status of best fit line


Link: 
https://www.udemy.com/course/pytorch-for-deep-learning-with-python-bootcamp/


### Autoencoder implementation in Linear way & in Convoluted way
I have attached a question paper here. And on the basis of this, I have developed a model for retain the provided architecture:

![](images/Question1.jfif)

I have tried to develop autoencoder on MNIST Dataset. For both way, I have followed the same approach. Both differs only in architecture of the model.

Steps:
1. Attaching Libraries
2. Collecting MNIST Dataset
3. 64 Batchsize data is separated from the dataset in dataloader where shuffle is false.
4. Go through to each data item of dataloader; here data item refers to images and labels; Normalized value
5. Model class with given architecture
6. get summary of model
7. Calculate MSE loss and Apply Adam optimizer
8. run the model for 20 epochs;
9. Get the results after the epoch at 0th, 4th, 8th and 16th. Compare them with the original data.

Link:
https://www.youtube.com/watch?v=zp8clK9yCro&t=184s

For more understanding and details, You can look over the code itself.



