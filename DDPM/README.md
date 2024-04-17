This is a from-scratch implementation of the original DDPM [paper]((https://arxiv.org/abs/1505.04597)). It is a notebook with the UNet model, the diffusion model, a training script, and an image generation script. This is a vanilla implementation - a linear, fixed noise schedule is used and there is no conditioning. The dataset used is the Fashion MNIST but you can use your own. 

From the original UNet, some things were changed - lesser residual blocks were used in the ascending & descending arms and I've also skipped the implementation of the attention block.

In the training script, I've extracted only 500 random images as a sanity check to see if the model overfits since I don't have the compute to train for more epochs or for longer. You can experiment with different training parameters, different noise schedulers.

For further reading, I recommend:
- Lilian Weng's [blog'(https://lilianweng.github.io/posts/2021-07-11-diffusion-models/)
- fast.ai's [video](https://www.youtube.com/watch?v=mYpjmM7O-30) explaining the math and in general, the entire course.
