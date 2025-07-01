# SVM - Support Vector Machine

- Hard Margin SVM
  - Loss Function
- Soft Margin SVM
  - Hinge Loss Function
  - Bias Variance Affects
- Constrained Optimization Problem
  - Gradient Vector Field
  - Lagrange's Multiplier
- SVM Dual Problem
- Converting From Primal form to Dual form
- Constraint Optimization with inequalities
  - Karush Kuhn Tucker Conditions
  - Concept of Duality
  - Dual Form
- Kernel SVM
  - Polynomial Kernel
  - RBF Kernel
  - Relationship between RBF and Polynomial Kernel
  - More forms of Kernels


**Summary for whole SVM Concept**

In SVM, the goal is to maximize the margin between two classes by finding the optimal hyperplane. The problem can be formulated as a primal optimization problem where we directly try to minimize a loss function that includes a margin constraint.

However, solving this primal form directly can be inefficient, especially when dealing with constraints. To transform it, we use Lagrange multipliers – a mathematical technique that helps convert optimization problems with constraints into another form, called the dual form.

In the dual form, the optimization problem becomes one of maximizing or minimizing with respect to the Lagrange multipliers rather than the original parameters (weights and biases). This new formulation depends only on the dot products between data points, which is computationally simpler. Another benefit is that this form allows us to apply kernel functions. Kernels replace the dot products with non-linear transformations, enabling SVM to work in higher dimensions where the data is more easily separable without actually having to compute those higher dimensions explicitly.

This dual form is therefore more efficient and makes SVM highly flexible by enabling non-linear boundaries, especially when using the kernel trick.
