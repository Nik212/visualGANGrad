#Visualizing gradient directions of generative models

This is the repository dedicated to a course project done for Machine Learning course at Skolkovo Institute of Science and Technology. 

Generative Adversarial Generative Adversarial networks are the models to implicitly sample from data distribution. Let $\mathbb{S}$ be some simple latent $H$-dimensional distribution, e.g. Gaussian. Let $\mathbb{Q}$ be the data distribution, e.g. aligned images of faces of CelebA64 dataset. GANs train a generator neural network $g_{\theta}$ to take as input samples from $\mathbb{S}$ and transform them to $\mathbb{Q}$. The training is done via minimizing some discrepancy between the generated and the true distribution w.r.t parameters $\theta$, i.e.
$$
D\left(g_{\theta} \sharp \mathbb{S}, \mathbb{Q}\right) \rightarrow \min _{\theta} .
$$
