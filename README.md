# Genetic_Algorithms
Genetic Optimization Using Derivatives


genoud is an R function that combines evolutionary algorithm methods with a derivativebased (quasi-Newton) method to solve difficult optimization problems. genoud may also
be used for optimization problems for which derivatives do not exist. genoud solves problems that are nonlinear or perhaps even discontinuous in the parameters of the function
to be optimized. When the function to be optimized (for example, a log-likelihood) is
nonlinear in the model’s parameters, the function will generally not be globally concave
and may have irregularities such as saddlepoints or discontinuities. Optimization methods
that rely on derivatives of the objective function may be unable to find any optimum at
all. Multiple local optima may exist, so that there is no guarantee that a derivative-based
method will converge to the global optimum. On the other hand, algorithms that do not
use derivative information (such as pure genetic algorithms) are for many problems needlessly poor at local hill climbing. Most statistical problems are regular in a neighborhood
of the solution. Therefore, for some portion of the search space, derivative information is
useful. The function supports parallel processing on multiple CPUs on a single machine
or a cluster of computers.
