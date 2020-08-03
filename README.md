# ICML 2020 Notes

## Representation Learning

1. [Distance Metric Learning with Joint Representation Diversification](https://proceedings.icml.cc/static/paper_files/icml/2020/4066-Paper.pdf): i). propose a Distance Metric Learning with Joint Representation Diversification (JRD) that allows a better balancing point between intra-class compactness and inter-class separability (which composed by [AMSoftmax](https://arxiv.org/abs/1801.09414) loss and the proposed JRS regularizer); ii). propose a Joint Representation Similarity regularizer (kernel inner product of output of layers with sample pairs from different classes) that captures different abstract levels of invariant features and diversifies the joint distributions of representations across multiple layer.


2. [Understanding Contrastive Representation Learning through Alignment and Uniformity on the Hypersphere](https://proceedings.icml.cc/static/paper_files/icml/2020/5503-Paper.pdf): identify two key properties related to the contrastive loss: (a) alignment (closeness) of features from positive pairs, and (b) uniformity of the induced distribution of the (normalized) features on the hypersphere.

3. [Unraveling Meta-Learning: Understanding Feature Representations for Few-Shot Tasks](https://arxiv.org/pdf/2002.06753.pdf): suggest meta-learning models can get better feature extractors and develop two measures for performance of extracted features: feature clustering and hyperplane variation, which actually show meta-learning can get feature spaces with larger margins. 

## Continual Learning  

1. [Optimal Continual Learning has Perfect Memory and is NP-HARD](https://proceedings.icml.cc/static/paper_files/icml/2020/204-Paper.pdf): main finding is that such optimal CL algorithms generally solve an NP-HARD problem and will require perfect memory to do so, also explain the excellent performance of CL algorithms using experience replay, episodic memory and core sets relative to regularization-based approaches.


2. [Online Continual Learning from Imbalanced Data](https://proceedings.icml.cc/static/paper_files/icml/2020/4727-Paper.pdf): basically like BER with reservoir sampling. 

3. [Model Fusion with Kullback–Leibler Divergence](https://arxiv.org/pdf/2007.06168.pdf): propose a method to fuse posterior distributions learned from heterogeneous datasets, which may be possible applied in continual learning as we can train a separate model for each task and the then fuse it with previously obtained model.

4. [LEEP: A New Measure to Evaluate Transferability of Learned Representations](https://proceedings.icml.cc/static/paper_files/icml/2020/3080-Paper.pdf): Log Expected Empirical Prediction (LEEP) requires a classifier trained on the source dataset and compute the average log-likelihood of the classifier on a target dataset, it can predict the performance and convergence speed of both transfer and meta-transfer learning methods. 

## Generalization

1. [Revisiting Training Strategies and Generalization Performance in Deep Metric Learning](https://proceedings.icml.cc/static/paper_files/icml/2020/1739-Paper.pdf): revisit the most widely used DML objective functions and conduct a study of the crucial parameter choices as well as the commonly neglected mini-batch sampling process, uncover a strong correlation between generalization performance in DML and the level of compression of learned data representation. 

2. [Fine-Grained Analysis of Stability and Generalization for Stochastic Gradient Descent](https://proceedings.icml.cc/static/paper_files/icml/2020/1028-Paper.pdf): gives the first-ever-known stability and generalization bounds for SGD with non-smooth loss functions (removing the existing bounded gradient  assumptions). 

3. [Rethinking Bias-Variance Trade-off for Generalization of Neural Networks](https://proceedings.icml.cc/static/paper_files/icml/2020/2946-Paper.pdf): for neural networks and other over-parameterized models, while the bias is monotonically decreasing as in the classical theory, the variance is unimodal or bell-shaped: it increases then decreases with the width of the network; evaluation on out-of distribution data shows that most of the drop in accuracy comes from increased bias while variance increases by a relatively small amount.


## Meta Learning

1. [TASKNORM: Rethinking Batch Normalization for Meta-Learning](https://arxiv.org/pdf/2003.03284.pdf): to normalize a task with the context set moments in combination with a set of non-transductive, secondary moments computed from the input being normalized, which is by the intuition that the normalization statistics µ and σ should be local at the task level.  


## Bayesian Inference

1. [How Good is the Bayes Posterior in Deep Neural Networks Really?](https://proceedings.icml.cc/static/paper_files/icml/2020/3581-Paper.pdf):  demonstrate through careful MCMC sampling that the posterior predictive induced by the Bayes posterior yields systematically worse predictions compared to simpler methods including point estimates obtained from SGD, demonstrate that predictive performance is improved significantly through the use of a “cold posterior” that overcounts evidence. 