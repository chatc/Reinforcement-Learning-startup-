# Reinforcement-Learning-startup

This is my repo of RL learning

*Value function*
$$
V^\pi(x)=\mathbb{E}\left[\sum_{t=0}^\infty\gamma^tR_{t+1}\Big| X_0=x\right],\quad x\in\chi
$$
*optimal action-value function*
$$
Q^*(x,a)=r(x,a) + \gamma\sum_{y\in\chi}\mathcal{P}(x,a,y)V^*(y),\quad  x\in\chi,a\in\mathcal{A}
$$
$\pi$ is optimal if for every $x\in\chi$ ,
$$
\sum_{a\in\mathcal{A}}\pi(a|x)Q^*(x,a)=V^*(x)
$$
*Bellman Equations for Deterministic Policies*
$$
    V^\pi(x) = r(x, \pi(x))+\gamma\sum_{y\in\chi}\mathcal{P}(x,\pi(x),y)V^\pi(y),\quad x\in\chi
$$