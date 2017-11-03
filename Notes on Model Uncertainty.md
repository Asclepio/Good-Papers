Notes on Model Uncertainty (Regarding to Bayesian Deep Learning)

1. Edward = TensorFlow + Random Variables + Inference Algorithms

2. Deep neural networks: many parameters; very prone to overfitting; require large data sets

3. Optimising any neural network with dropout is equivalent to a form of approximate Bayesian inference

4. A network trained with dropout already is a Bayesian Neural Network!

5. "typical training of neural networks requires lots of labeled data to control the risk of overfitting. And the problem becomes harder when it comes to real world regression tasks. These tasks often have smaller training data to use, and the high-frequency characteristics of these data often makes neural networks easier to get trapped in overfitting." http://zhusuan.readthedocs.io/en/latest/bayesian_nn.html

6. "In BNN, the approximate distribution is usually further simplified by factorizing it into independent distributions for each weight layers (mean field approximation). This approximation creates larger bias and can be problematic in the deep neural network." https://becominghuman.ai/learning-note-dropout-in-recurrent-networks-part-1-57a9c19a2307

7. "Uncertainty in predictions: As we will see below, the Bayesian Neural Network informs us about the uncertainty in its predictions. I think uncertainty is an underappreciated concept in Machine Learning as it’s clearly important for real-world applications. But it could also be useful in training. For example, we could train the model specifically on samples it is most uncertain about" - http://docs.pymc.io/notebooks/bayesian_neural_network_advi.html

8. "Training neural networks has a general problem that the parameters can be stuck in a local minimum, which limits the model performance. Therefore, in the training process, we hope the model parameters have the ability to jump out of the local minimum area when stuck at it and search in a bigger space to find the global minimum" - http://zhusuan.readthedocs.io/en/latest/bayesian_nn.html

9. "This might seem silly for such a small expression, but one of the key ideas in Tensorflow is deferred execution: it's very cheap to build a large and complex expression, and when you want to evaluate it, the back-end (to which you connect with a Session) is able to schedule its execution more efficiently (e.g. executing independent parts in parallel and using GPUs)." - https://stackoverflow.com/questions/33633370/how-to-print-the-value-of-a-tensor-object-in-tensorflow

10. "Standard deep learning tools for regression and classification do not capture model uncertainty. In classification,
predictive probabilities obtained at the end of the pipeline (the softmax output) are often erroneously interpreted as model confidence." https://arxiv.org/pdf/1506.02142.pdf

11. "It has long been known that infinitely wide (single hidden layer) NNs with distributions placed over their weights
converge to Gaussian processes (Neal, 1995; Williams, 1997). This known relation is through a limit argument that
does not allow us to translate properties from the Gaussian process to finite NNs easily." http://proceedings.mlr.press/v48/gal16.pdf

12. "The most commonly used automatic differentiation packages in machine learning, Theano (Bastien et al., 2012), Torch (Collobert et al., 2002) and TensorFlow(Abadi et al., 2016) require learning a new syntax in which to express operations, each acting as a compiler for a restricted mini-language" https://www.cs.toronto.edu/~duvenaud/papers/blackbox.pdf

