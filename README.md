# ml-skill-proj
Perceptron, regression, matrix

1. Consider the perceptron in two dimensions: h(x) = sign(wTx) where w = [w0;w1;w2]T and x = [1; x1; x2]^{T}. Technically, x has three coordinates, but we call this perceptron two-dimensional because the rst coordinate is fixed at 1.

(a) Show that the regions on the plane where h(x) = +1 and h(x) = -1 are separated by a line. If we express this line by the equation x2 = ax1 + b, what are the slope a and intercept b in terms of w0,w1,w2?
(b) Draw pictures for the cases w = [1; 2; 3]T and w = 􀀀[1; 2; 3]T . Label the positive and negative prediction regions on the pictures.

2.In logistic regression (labels are f1, -1g), the objective function can be written as 

![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/5e9f9ade-e229-42e7-9402-f76b032f4095)


(a) Compute the first-order derivative ∇ E(w). 
(b) Once the optimal w is obtain, it will be used to make predictions as follows:
![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/74878aa3-785b-4427-adee-aab662667742)

Explain why the decision boundary of logistic regression is still linear, though the linear signal wTx is passed through a nonlinear function θ
to compute the outcome of prediction.

(c) Is the decision boundary still linear if the prediction rule is changed to the following?

![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/c8943446-7ad6-4023-8d05-37206fe6be2f)


(d) what is the essential property of logistic regression that results in the linear decision boundary?
![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/df6d6b6e-1587-4e35-b2b9-a47186f35013)

3.
![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/7b9818fe-0ea7-42de-b82c-5d02c0063613)


4.We show that maximizing log-likelihood is equivalent to minimizing RSS(w).
In particular,
![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/34dcc0f2-3e44-4dd7-bf2c-0ec53eb7779f)

(a) Please derive the optimal w and $\sigma^{\star}$.

(b) What do you observe from the optimal $\sigma^{\star}$?

5.Show that sigmoid function and softmax function are the same in the binary case.
![image](https://github.com/jasmineyliang/ml-skill-proj/assets/150869870/fb6d5552-523e-4c13-943f-d0b649b2b423)

6. Perceptron for Handwritten Digits Recognition: The handwritten digits les are
in the \data" folder: train.txt and test.txt. The starting code is in the \code" folder. In the data
le, each row is a data example. The rst entry is the digit label (\1" or \5"), and the next 256
are grayscale values between -1 and 1. The 256 pixels correspond to a 16 x 16 image. You are
expected to implement your solution based on the given codes. The only le you need to modify
is the \solution.py" le. You can test your solution by running \main.py" le. Note that code is
provided to compute a two-dimensional feature (symmetry and average intensity) from each digit
image; that is, each digit image is represented by a two-dimensional vector before being augmented
with a \1" to form a three-dimensional vector as discussed in class. These features along with the
corresponding labels should serve as inputs to your Perceptron algorithm.

(a) complete the show images function. Include the images plotted in report.

(b) complete the show images function and include the 2-D scatter plot into report. For each sample, plot the two features with a red if the label is 1 and a blue + if the label is 5.

(c) Complete the Perceptron class, test accuracy results using the "test_accuracy" function in main.py.

(d) Complete the show result function to plot the test data with the separators. Include the images you plotted into your report.
