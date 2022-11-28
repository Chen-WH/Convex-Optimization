# L2_Convex sets

## affine and convex sets

- affine set: solution set of a set of linear equations
- convex set: $\forall x_1,x_2\in C,\forall \theta\in[0,1],\theta x_1+(1-\theta)x_2\in C$
- Convex combination: $\theta_1x_1+\theta_2x_2+\cdots+\theta_kx_k,\theta_1+\cdots+\theta_k=1,\theta_i\geq0$
- convex hull 凸包

## some important examples

- conic combination: $x=\theta_1x_1+\theta_2x_2,\theta_1\geq0,\theta_2\geq0$
- convex cone: set that contains all conic combinations of points in the set
- hyperplanes: set of the forms $\{x|a^Tx=b\}$
- halfspaces: set of the form $\{x|a^Tx\leq b\}$
- Euclidean ball: $B(x_c,r)=\{x|\|x-x_c\|_2\leq r\}=\{x_c+ru|\|u\|_2\leq1\}$
- ellipsoid: set of the form $\{x|(x-x_c)^TP^{-1}(x-x_c)\leq1\}=\{x_c+Au|\|u\|_2\leq1\}$ with $P$ symmetric positive definite, $A$ square and nonsingular
- norm

$$
\|\boldsymbol{x}\|\geq0,\|\boldsymbol{x}\|=0\text{ if and only if } x=0\\
\|t\boldsymbol{x}\|=|t|\|\boldsymbol{x}\|\\
\|\boldsymbol{x}+\boldsymbol{y}\|\leq\|\boldsymbol{x}\|+\|\boldsymbol{y}\|
$$

- polyhedra: solution set of finitely many linear inequalities and equalities $Ax\leq b,Cx=d$
- $S_+^n$ positive semidefinite $n\times n$ matrices (convex cone); $S_{++}^n$ positive definite

## operations that preserve convexity

- intersection
- affine function: scaling, translation, projection; solution set of linear matrix inequality; hyperbolic cone
- perspective: $P(x,t)=x/t,t>0$
- linear-fractional function: $f(x)=(Ax+b)/(c^Tx+d),c^Tx+d>0$

## generalized inequalities

- generalized inequality defined by a proper cone $K$: $x\leq_K y\Longleftrightarrow y-x\in K$
- minimum and minimal elements: $\forall y\in S,x\leq_K y$

## separating and supporting hyperplanes

- separating hyperplane theorem: the hyperplane $\{x|a^Tx=b\}$ separates $C$ and $D$ $a^Tx\leq b,\forall x\in C;a^Tx\geq b,\forall x\in D$
- supporting hyperplane: $\{x|a^Tx=a^Tx_0\},a^Tx\leq a^Tx_0,\forall x\in C$
- supporting hyperplane theorem: if $C$ is convex, then there exists a supporting hyperplane at every boundary point of $C$

## dual cones and generalized inequalities

- dual cone of a cone $K$: $K^*=\{y|(x,y)\geq0,\forall x\in K\}$
- dual cones of proper cones are proper, hence define generalized inequalities: $y\geq_{K^*}0\Longleftrightarrow y^Tx\geq0,\forall x\geq_K0$
