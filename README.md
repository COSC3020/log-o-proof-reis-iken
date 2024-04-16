[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/fbkbKZ5N)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$

**Given this definition for big O, we need to be able to prove that $O(\log_{2} n)$ is the same as $O(\log_{5} n)$.**

**This means that we must find constants $c_1$ and $c_2$ as well as $n_0$ such that $(\log_{2} n) \leq c_1 * (\log_{5} n) \forall n\geq n_0$**
**and**
**$(\log_{5} n) \leq c_2 * (\log_{2} n) \forall n\geq n_0$**

**In the first inequality $(\log_{2} n) \leq c_1 * (\log_{5} n)$ we can take the log of both sides and then simplify to get:**

**$n^{\log_{2} 5} \geq c_1$**

**And in the second inequality $(\log_{5} n) \leq c_2 * (\log_{2} n)$ we can once again take the log of both sides and then simplify to get:**

**$n^{\log_{5} 2} \geq c_2$**

**Since the left sides of both inequalities are increasing functions with respect to n, then we can choose $n_0$ = 1 as well as positive values for $c_1$ and $c_2$ that make the inequalities true for all n $\geq n_0$**
