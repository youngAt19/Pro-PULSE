# Pro-PULSE: Learning Progressive Encoders of Latent Semantics in GANs for Photo Upsampling
>The state-of-the-art photo upsampling method, PULSE, demonstrates that a sharp, high-resolution (HR) version of a given low-resolution (LR) input can be obtained by exploring the latent space of generative models. However, mapping an extreme LR input ($16^2$) directly to an HR image ($1024^2$) is too ambiguous to preserve faithful local facial semantics. In this paper, we propose an enhanced upsampling approach, Pro-PULSE, that addresses the issues of semantic inconsistency and optimization complexity. Our idea is to learn an encoder that progressively constructs the HR latent codes in the extended $W+$ latent space of StyleGAN. This design divides the complex 64$\times$ upsampling problem into several steps, and therefore small-scale facial semantics can be inherited from one end to the other. In particular, we train two encoders, the base encoder maps latent vectors in $W$ space and serves as a foundation of the HR latent vector, while the second scale-specific encoder performed in $W+$ space gradually replaces the previous vector produced by the base encoder at each scale. This process produces intermediate side-outputs, which injects deep supervision into the training of encoder. Extensive experiments demonstrate superiorities over the latest latent space exploration methods, in terms of efficiency, quantitative quality metrics, and qualitative visual results.
