#### Goal of training:
Given a probability density function p(x), its score function is defined as the gradient of the log probability density ∇x log p (x). A noise-conditional score network is a deep neural network sθ (x, t) trained to estimate the score function ∇x t log q(x t ). 
###### So: 

Trying to minimize some loss function involving the difference: $$ \nabla_{x_t} \log q(x_t) - s_{\theta}(x, t)  $$
### Score SDEs:
Score SDEs perturb data to noise with a diffusion process governed by the following stochastic differential equation (SDE):
$$ dx =  f (x, t)dt + g(t)dw $$
Where f (x,t) and g(t) are diffusion and drift functions of the SDE, and w is a standard Wiener process (a.k.a., Brownian motion).

#### Connection with Score Diffusion models

Crucially, for any diffusion process in the form of Eq. (15), Anderson [4] shows that it can be reversed by solving the following reverse-time SDE:

$$ dx =[f (x, t) − {g(t)}^2\nabla{_x} log(q_t(x))]dt + g(t)dw $$
