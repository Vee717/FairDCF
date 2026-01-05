# Learning Fair Graph Representations without Sensitive Attributes
Graph Neural Networks (GNNs) are widely deployed in real-world applications, yet their message-passing mechanisms can inherit 
and amplify latent biases in the data, leading to unfair predictions.Most existing fair graph learning methods rely on explicit
sensitive attributes for regularization or counterfactual modeling, which are often unavailable in practice due to privacy, legal, 
and ethical constraints. To address this issue, we propose FairDCF, a decoupled counterfactual fairness framework for graph learning 
that does not require access to sensitive attributes. Leveraging the dependency-sensitive properties of Graph Convolutional Networks (GCNs), 
FairDCF adopts a variational graph autoencoder framework with GCN-based encoders that jointly model task-relevant features and infer
pseudo-sensitive attributes from graph structure. Based on this formulation, FairDCF further applies a counterfactual strategy that
decouples node information prior to perturbing the inferred pseudo-sensitive attributes. To learn fair graph representations,
FairDCF enforces consistency constraints in both the representation and prediction spaces, ensuring invariance under counterfactual changes in sensitive attributes.
Extensive experiments on multiple real-world benchmark datasets demonstrate that FairDCF achieves competitive or superior predictive performance compared to existing methods, while effectively ensuring group fairness.

<p align="center">
  <img src="hmodel.png" width="550" title="hover text">
</p>
