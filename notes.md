# Construction of Reals
* Cauchy Sequences
* Dedekind Cuts

# Metric
## definition
For a set $X\ne\phi$ , a metric $d$ is a map
$d: X\rightarrow \mathbb{R}_ 0 ^+$ satisfying:
* d(x,y)=d(y,x)
* d(x,y)=0 $\iff$ x=y
* d(x,y) $\le$ d(x,z) + d(z,y)

## examples
* The p norm induced metric on Euclidean space $\mathbb{R}^n$, $(\Sigma_1^n |x_i-y_i|^p)^{1/p}$ , with $n,p \in \mathbb{N}$
* The discrete metric on any set X, $1$ for $x \ne$ y, $0$ otherwise.
* Supremum norm on Euclidean space $\mathbb{R}^n$, $sup_{i\in [n]} |x_i-y_i|$
# Bolzano Weirstrass Thm
## proposition
Any bounded sequence in $\mathbb{R}^n$ has a convergent subsequence
## proof

monotone convergence theorem on each component

or

nested intervals

# Kakeya Needle Problem
# Bounded Metric Space
**diameter**, $diam(X)=sup\{d(x,y) | x,y \in X\}$ is bounded.
# Open Ball
$B_r(x)=\{y \in X | d(x,y)\lt r\}$
# Closed Ball
$B_r(x)=\{y \in X | d(x,y)\le r\}$
# Convergence
for a sequence $\{x_n\}\rightarrow x$ means that $\forall \epsilon \gt 0\ \exists N\in \mathbb{N}$ such that $x_n \in B_{\epsilon}(x)\ \forall n \ge N$
# Cauchy Sequences
a sequence $\{x_n\}$ is cauchy means that $\forall \epsilon \gt 0\ \exists N\in \mathbb{N}$ such that $d(x_n,x_m)\lt \epsilon\ \forall n,m \ge N$
# Equivalent Metrics
TFAE
1. generate the same convergent sequences
2. generate the open sets
3. generate the same closed sets
4. generate the same continous maps

# Normed Linear Spaces
## Norm
map $||x|| : X\rightarrow \mathbb{R} _ 0^+$ on a vector space X
## norm induced metric
$d(x,y)=||x-y||$

## metric induced norm
$||x||=d(x,0_X)$


# Product of Metrics
## Given
Two metric spaces $(X,d_1)$ & $(Y,d_2)$
## Aim
Construct a metric $\rho$ on $X\times Y$ such that $(x_n,y_n)$ converges in $X \times Y \iff x_n$ converges in $X$ and $y_n$ converges in $Y$
## Choices
1. Root of p-Summation
2. Maximum
# Function and Sequence Spaces
## p-summable sequences
$\Sigma|x_i|^p\lt \infty$
### norm
$||\{x_n\}||_ p=$ $(\Sigma|x_i|^p)^{1/p}$
## Normed Linear Space of Continous Functions
$\mathscr{C}[a,b]$ $:=\{f:[a,b]\rightarrow \mathbb{R}, continous\}$
$||f_p||=(\int_a^b|f(x)|^pdx)^{1/p}$
# Equivalent Norms
TFAE
1. induce equivalent norms
2. generate same sequences converging to 0
# Open sets
TFAE
1. $\forall x \in U$ $\exists \epsilon \gt 0$ such that $B_{\epsilon}(x)\subseteq U$
2. for a sequence $x_n$ in $X$ converging to  $u \in U$ all but finitely many points lie in $U$
3. $U^C$ is closed in $X$
# Closed Sets
1. $x \in X$ such that $\forall \epsilon \gt 0$  $B_{\epsilon}(x)\cap V \ne \phi$,  $x \in V$
2. for any sequence $x_n$ in $V$ converging to a $v \in X$ we have  $v\in V$.
3. $V^C$ is open in $X$
# Distance of a point from a Set
$ A,B \subseteq X$, $x \in X$

$d(x,A)=inf\{d(x,y)\ | \ y\in A\}$

$d(A,B)=inf\{d(x,y)\ | x\in A\  \ y\in B\}$
## relation to point distances

$|d(x,A)-d(y,A)|\le d(x,y)$


# Dense Set
$A\subseteq X$ is said to be dense in $X$ if $closure(A)=\bar{A}=X$
# Nowhere dense Set
TFAE
1.
2.
3.
# Seperable space
$ (X,d)$ is said to be seperable if it has a **countable** dense subset.
# Interior, Closure, Boundary
## Defs
* Interior:= $\{x \in A\ | \exists \epsilon$ such that $B_{\epsilon}(x)\subseteq A \}$, largest open set contained in A
* Closure:= $A \cup \{a\ |\ \exists\ \{x_n\in A\} \rightarrow a\in X\}$, smallest closed set containing A
* Boundary:= $\{a\ |\ \exists\ \epsilon$ with $B_{\epsilon}(a)\cap A \ne \phi$ or $B_{\epsilon}(a)\cap A^C \ne \phi\}$, limit points of either $A$ or $A^C$
## a relation
$X=int(A)+int(A^C)+\delta(A)$
# Inequalities
## Young's
## Holder's  
## Minkowsky's
# Relative Openness
$A$ is open in $Y \iff \exists\ U$, open in $X$ such that $A=U\cap Y$
# Relative Closedness
$A$ is closed in $Y \iff \exists\ V$, closed in $X$ such that $A=V\cap Y$
# Continuity
$f: (X,d_1)\rightarrow (y,d_2)$ is said to be continous at $x\in X$ if TFE conditions hold
1. $\forall \epsilon\gt 0$ $\exists\ \delta\gt 0$ such that $f(B^{d_1}_ {\delta}(x))\subseteq B^{d_2}_ {\epsilon}(f(x)) )$
2. $x_n \rightarrow^{d_1} x$ $\implies$ $f(x_n) \rightarrow^{d_2} f(x)$
3. Inverse Image of closed set is closed.
4. Inverse Image of open set is open.

# Homomorphism
continous bijection
# Isometry
distance preserving continous injection
# Disconnectedness
if $\exists$ a seperation $(U,V)$, i.e. disjoint open sets such that $U\bigsqcup V=X$ 
# Interval characteriztion
if $a\in I \land b\in I$ then if $\forall c$ such that $a\lt c\lt b$ we have $c\in I$, then $I$ is called an **Interval**
