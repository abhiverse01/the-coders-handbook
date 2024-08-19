# Core Concepts to understand AI:

- Here’s a detailed list of core concepts in AI that are essential to master:

### 1. **Embeddings**
   - **Word Embeddings (Word2Vec, GloVe):** Techniques to convert words into continuous vectors in a lower-dimensional space, capturing semantic relationships.
   - **Sentence Embeddings (Sentence-BERT):** Extending word embeddings to entire sentences, allowing for semantic comparisons between sentences.
   - **Image Embeddings (ResNet, VGG):** Converting images into vector representations that capture visual features, often using pre-trained convolutional neural networks.
   - **Graph Embeddings (Node2Vec, GraphSAGE):** Representing nodes in a graph as vectors while preserving the graph structure.

### 2. **Attention Mechanisms**
   - **Self-Attention:** The core component of Transformer models, allowing the model to weigh the importance of different words in a sequence relative to each other.
   - **Multi-Head Attention:** Extending self-attention by using multiple attention heads, enabling the model to focus on different parts of the sequence simultaneously.
   - **Scaled Dot-Product Attention:** A specific implementation of attention used in Transformers, calculating the attention weights between queries, keys, and values.

### 3. **Transformers**
   - **Encoder-Decoder Architecture:** The foundational structure of Transformer models, used in tasks like machine translation.
   - **Positional Encoding:** Technique used in Transformers to encode the position of words in a sequence since the model lacks a built-in sense of order.
   - **BERT (Bidirectional Encoder Representations from Transformers):** A pre-trained Transformer model designed to understand the context of a word from both directions.
   - **GPT (Generative Pre-trained Transformer):** A Transformer model focused on generating coherent text, using a unidirectional approach.

### 4. **Convolutional Neural Networks (CNNs)**
   - **Convolutional Layers:** Layers that apply filters to input data, primarily used for image processing.
   - **Pooling Layers (MaxPooling, AveragePooling):** Downsampling techniques that reduce the spatial dimensions of feature maps while retaining important features.
   - **Fully Connected Layers:** Layers where each neuron is connected to every neuron in the previous layer, typically used at the end of CNNs for classification.
   - **Transfer Learning in CNNs (Fine-Tuning Pre-Trained Models):** Adapting a pre-trained CNN to a new task by fine-tuning some or all layers.

### 5. **Recurrent Neural Networks (RNNs)**
   - **Vanilla RNN:** A basic RNN where each neuron has a connection back to itself, allowing for the processing of sequential data.
   - **Long Short-Term Memory (LSTM):** An RNN variant designed to handle long-range dependencies using gates to control the flow of information.
   - **Gated Recurrent Unit (GRU):** A simpler alternative to LSTM with fewer parameters, also used for handling long-term dependencies.
   - **Bidirectional RNN:** An RNN where the sequence is processed in both directions, improving context understanding.

### 6. **Reinforcement Learning (RL)**
   - **Markov Decision Processes (MDPs):** A mathematical framework for modeling decision-making where outcomes are partly random and partly under the control of a decision-maker.
   - **Q-Learning:** An off-policy RL algorithm where the agent learns a value function that estimates the total reward it can obtain from each state-action pair.
   - **Deep Q-Networks (DQN):** Combining Q-learning with deep neural networks to handle environments with high-dimensional state spaces.
   - **Policy Gradients:** An RL method where the agent directly optimizes the policy by adjusting the parameters in the direction of higher rewards.
   - **Actor-Critic Methods:** A hybrid approach combining policy gradients (actor) and value function estimation (critic) to stabilize training.

### 7. **Generative Models**
   - **Generative Adversarial Networks (GANs):** A framework where two neural networks (generator and discriminator) are trained simultaneously, with the generator producing realistic data and the discriminator trying to distinguish between real and fake data.
   - **Variational Autoencoders (VAEs):** A generative model that learns to encode input data into a latent space and decode it back, allowing for the generation of new data by sampling from the latent space.
   - **Normalizing Flows:** A method for constructing complex probability distributions by transforming simple ones using invertible functions.

### 8. **Graph Neural Networks (GNNs)**
   - **Graph Convolutional Networks (GCNs):** Extending CNNs to graph-structured data by applying convolutions over nodes and their neighbors.
   - **Graph Attention Networks (GATs):** Applying attention mechanisms to GNNs, allowing the model to weigh the importance of different neighbors for each node.
   - **Message Passing:** A key operation in GNNs where information is passed between nodes based on their edges, allowing the network to capture dependencies between connected nodes.

### 9. **Bayesian Inference**
   - **Bayesian Networks:** A graphical model that represents probabilistic relationships among variables using directed acyclic graphs (DAGs).
   - **Markov Chain Monte Carlo (MCMC):** A method for sampling from probability distributions where direct sampling is difficult, often used in Bayesian inference.
   - **Variational Inference:** An approach for approximating complex probability distributions by optimizing a simpler distribution to be close to the target distribution.

### 10. **Optimization Techniques**
   - **Gradient Descent:** The core optimization algorithm used for training neural networks, where the model parameters are adjusted iteratively to minimize a loss function.
   - **Stochastic Gradient Descent (SGD):** A variant of gradient descent where only a subset of the data (a batch) is used to compute the gradient, improving computational efficiency.
   - **Adam Optimizer:** An adaptive learning rate optimization algorithm combining the benefits of Adagrad and RMSprop, widely used in deep learning.
   - **Learning Rate Schedulers:** Techniques to adjust the learning rate during training, such as reducing it on plateaus or using a cyclical schedule.

### 11. **AutoML and Neural Architecture Search (NAS)**
   - **Hyperparameter Optimization (Grid Search, Random Search, Bayesian Optimization):** Techniques for automatically searching the space of hyperparameters to find the best configuration for a model.
   - **Neural Architecture Search (NAS):** Methods for automatically designing neural network architectures optimized for a specific task, often using reinforcement learning or evolutionary algorithms.
   - **AutoML Frameworks (AutoKeras, Auto-sklearn):** Tools that automate the end-to-end process of applying machine learning to real-world problems.

### 12. **Explainability and Interpretability**
   - **SHAP (SHapley Additive exPlanations):** A method for explaining the output of machine learning models by attributing contributions to each feature.
   - **LIME (Local Interpretable Model-agnostic Explanations):** A technique to explain individual predictions by approximating the model locally with an interpretable model.
   - **Saliency Maps:** Visualization techniques used primarily in CNNs to highlight which parts of the input image contribute most to the model’s prediction.
   - **Attention Visualization:** Techniques to visualize the attention weights in models like Transformers, helping to understand which parts of the input the model focuses on.

### 13. **Transfer Learning**
   - **Fine-Tuning Pre-Trained Models:** The process of adapting a pre-trained model to a new task by training it further on a smaller dataset specific to the task.
   - **Domain Adaptation:** Techniques to adapt a model trained in one domain (e.g., image classification) to work in another domain (e.g., medical imaging) with minimal retraining.
   - **Zero-Shot Learning:** A form of transfer learning where the model is able to generalize to new classes that it hasn’t seen during training.

### 14. **Federated Learning**
   - **Client-Server Architecture:** The foundational setup where multiple clients train models on local data and send updates to a central server without sharing raw data.
   - **Model Aggregation:** Techniques to combine the locally trained models from multiple clients into a global model on the server.
   - **Privacy-Preserving Techniques (Differential Privacy, Secure Aggregation):** Methods to ensure that individual data points cannot be reconstructed or identified from the aggregated model.

### 15. **Temporal Graph Networks (TGNs)**
   - **Temporal Node Embeddings:** Methods to capture the evolving nature of nodes in dynamic graphs, allowing the model to account for changes over time.
   - **Memory Modules:** Components in TGNs that store historical information about nodes, enabling the model to retain context across time.
   - **Temporal Attention Mechanisms:** Techniques to weigh the importance of different time steps, ensuring the model focuses on relevant temporal information.

### 16. **Neural Differential Equations**
   - **ODE Networks (Neural ODEs):** A new class of models where the hidden state of a neural network is the solution to a differential equation, providing a continuous depth model.
   - **Adjoint Sensitivity Method:** A technique used in training neural ODEs to compute gradients efficiently by solving another differential equation backward in time.
   - **Applications of Neural ODEs:** Use cases in time series modeling, physics-informed neural networks, and beyond.

### 17. **Self-Supervised Learning**
   - **Contrastive Learning (SimCLR, MoCo):** A framework for learning useful representations by contrasting similar and dissimilar pairs of data points.
   - **Masked Language Modeling (BERT Pre-training):** A pre-training task where some percentage of the words in a sentence are masked, and the model must predict them.
   - **Rotation Prediction

:** An auxiliary task where the model is trained to predict the rotation applied to an image, encouraging the learning of robust visual features.

### 18. **Meta-Learning**
   - **Model-Agnostic Meta-Learning (MAML):** A method where the model is trained to quickly adapt to new tasks with only a few examples by learning good initialization parameters.
   - **Prototypical Networks:** A few-shot learning approach where the model learns a metric space in which classification can be performed by computing distances to prototype representations of each class.
   - **Reptile:** A simpler alternative to MAML, using first-order optimization techniques to achieve similar results with less computational overhead.

### 19. **Probabilistic Programming**
   - **Bayesian Neural Networks:** Neural networks where the weights are treated as distributions rather than fixed values, enabling uncertainty estimation in predictions.
   - **Probabilistic Programming Languages (Pyro, Stan):** Languages designed to specify probabilistic models and perform inference, often used in Bayesian statistics.
   - **Variational Autoencoders (VAEs) in Probabilistic Programming:** A use case of probabilistic models where the encoder maps data to a distribution in the latent space, and the decoder generates data from this distribution.

### 20. **Differentiable Programming**
   - **Autograd:** Automatic differentiation systems that compute gradients of functions expressed as code, enabling the training of complex models that include arbitrary computations.
   - **Universal Approximation with Neural Networks:** Theoretical foundation proving that neural networks can approximate any function given sufficient capacity.
   - **Neural Ordinary Differential Equations (ODEs):** Extending the idea of differentiable programming to model continuous-time dynamics, providing a more natural way to model time-dependent phenomena.

### 21. **Quantization and Model Compression**
   - **Weight Quantization:** Reducing the precision of the weights in a neural network to lower memory usage and computation cost.
   - **Knowledge Distillation:** A technique where a smaller "student" model is trained to mimic the behavior of a larger "teacher" model, reducing the size of the model while maintaining performance.
   - **Pruning:** Removing less important weights from a neural network to make it smaller and faster, often followed by fine-tuning.

### 22. **Neurosymbolic AI**
   - **Combining Neural Networks with Symbolic Reasoning:** Integrating deep learning models with rule-based symbolic AI to achieve better generalization and interpretability.
   - **Differentiable Programming for Symbolic Manipulation:** Applying differentiable programming to perform symbolic reasoning tasks, such as algebraic manipulation or logical inference.
   - **Applications in Neurosymbolic AI:** Use cases in question answering, reasoning over knowledge graphs, and automated theorem proving.

### 23. **Adversarial Machine Learning**
   - **Adversarial Attacks (FGSM, PGD):** Techniques used to fool machine learning models by making subtle changes to the input data that cause the model to make incorrect predictions.
   - **Adversarial Training:** A defense mechanism where models are trained on adversarial examples to improve their robustness against attacks.
   - **Robustness and Certification:** Techniques to quantify and certify the robustness of models against adversarial examples, ensuring that they perform reliably even under adversarial conditions.

### 24. **Causal Inference in AI**
   - **Causal Graphs:** Representing causal relationships between variables using directed acyclic graphs (DAGs), enabling causal reasoning and inference.
   - **Instrumental Variables:** A technique in causal inference used to estimate causal effects when controlled experiments are not feasible.
   - **Counterfactual Reasoning:** The process of reasoning about what would have happened under different circumstances, crucial for decision-making and policy analysis.

### 25. **Explainable AI (XAI) Techniques**
   - **Saliency Maps and Attention Visualization:** Techniques to visualize which parts of the input are most influential in a model’s prediction, improving interpretability.
   - **Post-Hoc Explanation Methods (LIME, SHAP):** Tools that provide explanations for individual predictions, making models more transparent.
   - **Rule-Based Explanations:** Techniques to extract logical rules from models, particularly decision trees and rule-based classifiers, to provide interpretable outputs.

These specific core concepts are crucial for building a deep understanding of AI and its applications. Mastering them enables one to design, implement, and optimize AI systems that are both powerful and efficient.
