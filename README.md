[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

The goal of this particular proof is to show that for any two functions $f(n)$ and $g(n)$, if $f(n)$ \in o(g(n))$ then $f(n)$ is also inculded within $O(g(n))$.

To do this we can look at a formal definition of $O$
$f(n)\in O(g(n)) \iff \exists c>0,n_0 >0, \forall n\ge n_0: f(n) \le c g(n)$

Looking at the two side by side, I only notice two differences. the first being that the definition of $o$ has the portion $\forall c>0$ whereas $O$ has $\exists c>0$. Thinking about this, the statement for all by default implies that there exists which makes a point for $o$ including $O$.

What I believe to be more important however, is that in $o$ there is a $<$ while in contrast, $O$ has a &\le&. When you add the "or equal to" portion to that end statement, it becomes more inclusive. My line of thought is that because the $O$ statement includes more with the $\le$ it proves that any $f(n)$ would be included in both $o$ and $O$.


