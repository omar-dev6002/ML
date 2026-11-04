# Chapter 1 — The Machine Learning Landscape: Exercises

## Q1. How would you define Machine Learning?
A computer program is said to learn from experience E with respect to
some class of tasks T and performance measure P, if its performance at
tasks in T, as measured by P, improves with experience E.

## Q2. Can you name four types of problems where it shines?
ML is great for complex problems for which we can't find an algorithmic
solution; to replace long lists of hand-tuned rules; to build systems that
adapt to fluctuating environments; and to help humans learn (data mining).

## Q3. What is a labeled training set?
A labeled training set is a training set that includes the desired output
(label) for each instance.

## Q4. What are the two most common supervised tasks?
Regression and classification.

## Q5. Can you name four common unsupervised tasks?
Clustering, visualization, dimensionality reduction, association rule
learning, and anomaly/novelty detection.

## Q6. What type of ML algorithm would you use to allow a robot to walk in various unknown terrains?
Reinforcement learning.

## Q7. What type of algorithm would you use to segment your customers into multiple groups?
Clustering (unsupervised) — or classification if you already know the
groups you want (supervised).

## Q8. Would you frame spam detection as supervised or unsupervised?
Supervised.

## Q9. What is an online learning system?
A learning system that can learn incrementally, as opposed to a batch
learning system. It is capable of adapting rapidly.

## Q10. What is out-of-core learning?
A type of algorithm that can handle vast quantities of data that cannot
fit in a computer's memory. It chops data into multiple small datasets
(mini-batches) and uses online learning techniques for these batches.

## Q11. What type of learning algorithm relies on a similarity measure to make predictions?
An instance-based learning system learns the training data by heart; then,
when given a new instance, it uses a similarity measure to find the most
similar learned instances to make predictions.

## Q12. What is the difference between a model parameter and a learning algorithm's hyperparameter?
A model has one or more model parameters that determine what it will
predict given a new instance. A learning algorithm tries to find the
optimal values for these parameters such that the model generalizes well
to new instances. A hyperparameter is a parameter of the learning
algorithm itself, not of the model (e.g., the amount of regularization to
apply).

## Q13. What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?
Model-based learning algorithms search for an optimal value for the model
parameters such that the model will generalize well to new instances. We
usually train such systems by minimizing a cost function (with a penalty
for model complexity if the model is regularized). To make predictions,
we feed the new instance's features into the model's prediction function,
using the parameter values found by the learning algorithm.

## Q14. Can you name four of the main challenges in Machine Learning?
Lack of data, poor data quality, non-representative data, uninformative
data, underfitting, and overfitting.

## Q15. If your model performs great on training data but generalizes poorly, what's happening? Name three solutions.
This is overfitting. Possible solutions: getting more data, simplifying
the model, reducing noise, reducing the number of parameters.

## Q16. What is a test set and why would you use it?
A test set is used to estimate the generalization error that a model will
make on new instances, before the model is launched in production.

## Q17. What is the purpose of a validation set?
A validation set is used to compare models and tune hyperparameters —
to select the best model and fine-tune the hyperparameters.

## Q18. What can go wrong if you tune hyperparameters using the test set?
There is a risk of overfitting, and the generalization error we measure
may be optimistic (the model performs worse than expected on truly
unseen data).

## Q19. What is cross-validation, and why would you prefer it to a validation set?
Cross-validation is a technique that makes it possible to compare models
(for model selection and hyperparameter tuning) without needing a
separate validation set. This saves training data.