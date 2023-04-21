# Chapt 11 Regression
The content was presented in the chapt 11 in FML book. In this Chapt,we
can learn some conclusions that wrere frequently used in Regression,especially in the Machine Learning.

We could learn:

- Generalization bounds, both in **finite** and  **infinite hypothesis sets**.

- Introduce the peseudo-dimension,which is the extension of VC-dim in Regression Background.

- Present some Regression algorithm,such as linear regression,kernel ridge regression,super-vector regression、lasso and their on-line versions.



## 11.1 The problem of Regression
Firstly, The $\mathcal{X}$ and $\mathcal{Y}$ represent the sample space and label space separtely, and denote $\mathcal{D}$ as the distribution
of $\mathcal{X} \times \mathcal{Y}$, learning the purposed function $f : \mathcal{X} \longrightarrow \mathcal{Y}$ is the algorithms' goal.

Secondly, we define the measure of error as our loss function. For instance, we construct $L:\mathcal{Y} \times \mathcal{Y} \longrightarrow \mathbb{D}$ ,beside tha, we define $L(y,y^{\prime}) = |y^{\prime} - y|^{p}$ as our typical loss function,and $p \geq 1$.

Thirdly, the hypothesis set $\mathcal{H}$ including the functions that mapping from $\mathcal{X}$ to $\mathcal{Y}$,based on the sample S,and $h \in \mathcal{H}$,we define the expected loss:
$$
   R(h) = \mathbb{E}_{(x,y) ~ \mathcal{D}}[L(h(x),y)]
$$
