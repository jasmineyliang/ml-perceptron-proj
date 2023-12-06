# ml-skill-proj
Perceptron, regression, matrix

1. Consider the perceptron in two dimensions: h(x) = sign(wTx) where w = [w0;w1;w2]T and x = [1; x1; x2]T . Technically, x has three coordinates, but we call this perceptron two-dimensional because the rst coordinate is fixed at 1.

(a) Show that the regions on the plane where h(x) = +1 and h(x) = -1 are separated by a line.
If we express this line by the equation x2 = ax1 + b, what are the slope a and intercept b in terms of w0,w1,w2?
(b) Draw pictures for the cases w = [1; 2; 3]T and w = 􀀀[1; 2; 3]T . Label the positive and negative prediction regions on the pictures.

2. We show that maximizing log-likelihood is equivalent to minimizing RSS(w).
In particular,
log L(w|x) = -1/2
1
2

1
2RSS(w) + n log 2

+ const
(a) (5 points) Please derive the optimal w and .
(b) (5 points) What do you observe from the optimal ?
