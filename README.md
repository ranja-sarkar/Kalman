
**Chapter 7** of my [book](https://a.co/d/1zUEkNQ) discusses the Kalman filter. The goal of a **state space model** is to infer information about the state variables of a dynamic system, given the observations. The algorithm for SSM is Kalman Filter.

<img width="174" alt="3" src="https://github.com/user-attachments/assets/6d8c55ba-1e33-48e4-976d-f69658fdb3c2">


# SSM

The state space representation of a time-series problem is a sequential analysis framework that typically includes tasks like filtering and smoothing. 

State space models (SSMs) are a class of machine learning algorithms used to make predictions about dynamic systems by modeling how their internal states evolve over time through differential equations. SSMs traditionally are used in control theory. Real-world data is discrete (recurrent) and discretization is one of the important (if not the most important) steps in SSM. 

While deterministic dynamics in discrete time can be handled by discretized ODEs/automata, stochastic dynamics of systems is tackled by SSMs. In SSMs, Kalman filter is the algorithm used to study the [state variables](https://hazyresearch.stanford.edu/blog/2022-01-14-s4-3) of the system evolving with time.


![00](https://github.com/user-attachments/assets/6719b226-816d-4e28-9635-cfe4fd0aac95)

Bayesian SSMs are typically used in macroeconometrics.

Find out more from another book: https://bookdown.org/rdpeng/timeseriesbook/state-space-models-and-the-kalman-filter.html
