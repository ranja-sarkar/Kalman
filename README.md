
Kalman Filter is discussed in **Chapter 7** of my [book](https://a.co/d/1zUEkNQ). As my book was published in the last quarter of 2023 and mamba arrived in 2024, the chapter doesn't discuss mamba models. 👇

The goal of a **state space model** is to infer information about the state variables of a dynamic system, given the observations. The algorithm underlying SSMs is Kalman Filter.

State space models have their origins in control systems engineering. Underpinning SSMs are two equations - one describes the internal dynamics of a system that aren’t directly observables, and the other describes how the internal dynamics relate to observable results. This formulation is extremely adaptable for a wide variety of multivariate time-series data.

# SSMs

State space models (SSMs) are a class of algorithms used to make predictions about dynamic systems by modeling how their internal states evolve over time through differential equations. SSMs traditionally are used in control theory. Real-world data is discrete (recurrent) and discretization is one of the important (if not the most important) steps in SSM. 

While deterministic dynamics in discrete time can be handled by discretized ODEs/automata, stochastic dynamics of systems is tackled by SSMs. Kalman filter is the algorithm in [SSMs](https://bookdown.org/rdpeng/timeseriesbook/state-space-models-and-the-kalman-filter.html) to study the [state variables](https://hazyresearch.stanford.edu/blog/2022-01-14-s4-3) of the system evolving with time.


![00](https://github.com/user-attachments/assets/6719b226-816d-4e28-9635-cfe4fd0aac95)

Bayesian SSMs are typically used in macroeconometrics.

The state space representation of a time-series problem is a sequential analysis framework that typically includes tasks like [filtering](https://github.com/ranja-sarkar/Kalman/blob/003791fbe4dd3f93aef5399575ace364c1a32f44/code/filtrate.py) and [smoothing](https://github.com/ranja-sarkar/Kalman/blob/003791fbe4dd3f93aef5399575ace364c1a32f44/code/compute.py). 

# Mamba

Mamba is a neural network architecture, derived from SSMs, used for language modeling and other sequence modeling tasks. The [Mamba architecture’s](https://arxiv.org/pdf/2312.00752) fast inference speed and computational efficiency, particularly for long sequences, make it the first competitive alternative to the transformer architecture for autoregressive LLMs.

<img width="367" height="344" alt="mamba" src="https://github.com/user-attachments/assets/2cefa706-69bb-48f5-bb91-7827c98a7f49" />

The procedure (x in the figure) following the selective SSM refers to element-wise multiplication, rather than standard dot product.

Mamba models are perhaps the first deep learning architecture to rival the efficacy of transformer models on the task for which they are originally known which is language modeling.


