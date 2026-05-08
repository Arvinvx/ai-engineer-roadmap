# Layer 4 — Deep ML Understanding

**Courses & Resources:**
- [IBM AI Engineering Professional Certificate](https://www.coursera.org/professional-certificates/ai-engineer) — Coursera
- [Neural Networks: Zero to Hero](https://www.youtube.com/playlist?list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ) — Andrej Karpathy
- [3Blue1Brown](https://www.youtube.com/@3blue1brown) — Visual math intuition

**Timeline:** Feb 2027 – Jun 2027  
**Goal:** Understand what's actually happening inside AI models — not just how to use them, but how they work.

---

## What You Learn

### 1. The Math That Underpins Everything (3Blue1Brown)

Before neural networks make sense, the math needs to click.

**Linear Algebra**
- Vectors and vector spaces — the geometry of data
- Matrix multiplication — what it actually means visually
- Dot products and their geometric interpretation
- Eigenvalues and eigenvectors — how PCA and attention relate
- Matrix transformations: rotations, scaling, projections

**Calculus**
- Derivatives as rates of change — the intuition, not just the rules
- The chain rule — why backpropagation works
- Partial derivatives and gradients — the direction of steepest ascent
- Gradient descent visualized — rolling down a loss landscape

**Probability & Statistics**
- Probability distributions: normal, uniform, softmax
- Bayes' theorem — how priors update with evidence
- Entropy and information — what "uncertainty" means mathematically
- Cross-entropy loss — why it's the right loss for classification

**Why it matters:** 3Blue1Brown makes this visual and intuitive. You stop treating math as formulas to memorize and start seeing it as the geometry behind how models learn.

---

### 2. Neural Networks from Scratch (Karpathy — Zero to Hero)

The most important ML curriculum on the internet. Build everything from scratch.

**micrograd — Backpropagation by Hand**
- Implement a scalar-valued autograd engine in ~100 lines of Python
- Understand the computation graph: nodes, edges, gradients
- Forward pass: computing outputs
- Backward pass: propagating gradients via the chain rule
- Why automatic differentiation is the engine of all deep learning

**makemore — Language Models from First Principles**
- Bigram language model: predicting the next character
- Multi-layer perceptron (MLP) character-level model
- Batch normalization: why training is unstable without it
- Embeddings: turning discrete tokens into continuous vectors
- Train/val/test splits and why they matter

**Building GPT from Scratch**
- Tokenization: byte-pair encoding, how text becomes tokens
- Self-attention: the core mechanism behind transformers
- Multi-head attention: attending to multiple representation subspaces
- Positional encoding: giving the model a sense of order
- The transformer block: attention + feedforward + residual connections + layer norm
- Scaling: what changes as models get bigger
- Training a character-level GPT on real text

**Why it matters:** This is the curriculum that removes the black box. After Karpathy's series, you can read the GPT-2 paper and understand every equation. That's a rare and valuable position.

---

### 3. Machine Learning Theory (IBM AI Engineering)

The formal engineering side of ML — algorithms, evaluation, and the full workflow.

**Classical ML Foundations**
- Supervised vs unsupervised vs reinforcement learning
- Linear regression: least squares, gradient descent formulation
- Logistic regression: the binary classification workhorse
- Decision trees and random forests: ensemble methods
- Support vector machines (SVMs): maximum margin classifiers
- k-means clustering and dimensionality reduction (PCA, t-SNE)
- Bias-variance tradeoff — overfitting, underfitting, regularization

**Deep Learning Engineering**
- Convolutional neural networks (CNNs): image understanding
- Recurrent neural networks (RNNs) and LSTMs: sequence modeling
- Transformers: architecture deep dive beyond what Karpathy covers
- Transfer learning and fine-tuning pre-trained models
- Loss functions: MSE, cross-entropy, contrastive loss
- Optimizers: SGD, Adam, AdamW — what they do differently
- Learning rate schedules: warmup, cosine decay

**Model Evaluation**
- Confusion matrix, precision, recall, F1 — when each matters
- ROC curves and AUC
- Train/validation/test discipline — data leakage and how to avoid it
- Cross-validation strategies
- Calibration: is the model's confidence actually reliable?

**Why it matters:** IBM's certificate gives the formal vocabulary and engineering rigour that Karpathy's hands-on series doesn't. Both are necessary — one teaches intuition, one teaches discipline.

---

### 4. MLOps — Getting Models to Production

Building models is 20% of the work. The other 80% is keeping them working.

- ML pipelines: data → training → evaluation → deployment
- Feature engineering and feature stores
- Model versioning with MLflow or Weights & Biases
- Containerizing ML workloads with Docker
- Model serving: REST APIs for inference (FastAPI + model)
- Batch vs real-time inference — when each makes sense
- Model monitoring: data drift, concept drift, performance degradation
- Retraining pipelines: automated triggers when performance drops
- A/B testing models in production

**Why it matters:** A model that isn't deployed helps no one. MLOps is the engineering discipline that closes the gap between "it works in a notebook" and "it's running in production serving real users."

---

### 5. Fine-Tuning & Adapting Models

Going beyond prompting — actually changing what a model knows.

- When fine-tuning beats RAG (and when it doesn't)
- Instruction fine-tuning: teaching a model to follow directions better
- Parameter-efficient fine-tuning (PEFT): LoRA and QLoRA
- Supervised fine-tuning (SFT) on custom datasets
- RLHF basics: reinforcement learning from human feedback
- Direct preference optimization (DPO): a simpler alternative to RLHF
- Evaluating fine-tuned models: benchmarks and human eval
- Quantization: running large models on smaller hardware

**Why it matters:** Fine-tuning is how you build AI products with genuine differentiation — models that behave in ways no amount of prompting could achieve.

---

## Skills Unlocked After This Layer

By the end of Layer 4, you can:

- Implement a transformer from scratch in Python — no magic, no black boxes
- Read and understand ML research papers
- Fine-tune open-source models on custom datasets
- Build and operate end-to-end ML pipelines in production
- Make informed decisions about model architecture, training, and deployment

---

## The Full Picture

After all four layers, you're a **Full-Stack AI Engineer** — someone who can:

- Build the backend infrastructure AI products run on (Layer 1)
- Integrate and ship AI features that users actually interact with (Layer 2)
- Design systems that scale to millions of users (Layer 3)
- Understand and adapt the models powering those features (Layer 4)

That's the goal.

**Previous:** [Layer 3 — Systems Thinking](layer3-systems.md)  
**Back to overview:** [Main README](../README.md)
