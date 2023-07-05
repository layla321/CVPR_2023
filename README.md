# CVPR 2023 (Virtual)
Notes and work related to the conference

## [Keynotes and Panels](https://cvpr.thecvf.com/virtual/2023/eventlistwithbios/2023KeynotesPanels)

- [Revisiting Old Ideas With Modern Hardware](https://cvpr.thecvf.com/virtual/2023/invited-talk/23301)
  - Great talk highlighting some of the history of CV and how old ideas returned as technology improved
  - Highlighted challenges with predicting where AI will go in the future
- [History and Future of Artificial Intelligence and Computer Vision](https://cvpr.thecvf.com/virtual/2023/panel/23304)
  - Historic look at the field and conference. Interesting to see how their perspective differed from mine, for example, I view this as a deep learning conference and they do not, at least not until recently. 
- [An AI Odyssey: the Dark Matter of Intelligence](https://cvpr.thecvf.com/virtual/2023/invited-talk/23302)
  - Talk on what is possible with AI and the limits of our current methods
- [Vision, Language, and Creativity](https://cvpr.thecvf.com/virtual/2023/panel/23305)
  - Discussion with creative experts like artists about how to involve them in computer vision
- [PAMI Meeting](https://cvpr.thecvf.com/virtual/2023/panel/23564)
  - Meeting to discuss how the conference was run and the future of CVF conferences like CVPR, ICCV, and ECCV among others 
- [Modeling Atoms to Address Our Climate Crisis](https://cvpr.thecvf.com/virtual/2023/invited-talk/23303)
  - Look at how to use CV to model the interaction of atoms 
- [Scientific Discovery and the Environment](https://cvpr.thecvf.com/virtual/2023/panel/23306)
  - Topics ranging from climate change to sub-atomic particles

## Tutorials and Workshops
- [Vision Transformer: More is Different](https://cvpr.thecvf.com/virtual/2023/tutorial/18572)
- [Recent Advances in Vision Foundation Models](https://cvpr.thecvf.com/virtual/2023/tutorial/18558)
- [Full-Stack, GPU-based Acceleration of Deep Learning](https://cvpr.thecvf.com/virtual/2023/tutorial/18561)
- [Large-Scale Visual Localization](https://cvpr.thecvf.com/virtual/2023/tutorial/18551)

## Papers and Posters

- [Visual Programming: Compositional Visual Reasoning Without Training](https://cvpr.thecvf.com/virtual/2023/poster/22652) - Best Paper Winner
  - Overview of a method for quickly writing code that reaches out to services like object detection to complete tasks like "change the car to be a BMW" without building an end-to-end model or creating unique services for each task.
  - How does it connect to those services?
- [A Generalized Framework for Video Instance Segmentation](https://cvpr.thecvf.com/virtual/2023/poster/22446)
  -  An approach to image segmentation that tries to make the training and inference data more similar. For example, training data often consists of very short video segments, potentially only a few frames, whereas inference videos can be minutes or hours.
- [Scaling Up GANs for Text-to-Image Synthesis](https://cvpr.thecvf.com/virtual/2023/poster/22519)
  - Why GANs? Is it for a speed improvement? Starting in 2022 diffusion models took over for this task
  - GANs only need a single forward pass for generation whereas diffusion models need an iterative denoising process
  - Using CLIP and a learned text encoder
  - Produces images of multiple sizes. Are they contrasted against one another as part of the generation process?
  - Can start with a low-res image and upscale it
  - Highlighted some failure cases to be aware of
- [On Distillation of Guided Diffusion Models](https://cvpr.thecvf.com/virtual/2023/poster/21256)
  - Classified-free guided diffusion models, like DALLE-2 and Stable Diffusion, consist of a guidance strength parameter and two diffusion models (an unconditional model and a conditional model)
  - CFG is necesssary for high-quality results
  - During each denoising step the models estimate the predicted noise, combining the two models
  - The downside is that they are computationally expense during inference since there are two models
  - This paper proposes a two-stage approach to distill the CFG models into a faster model for sampling
    - Stage 1: Guidance Distillation - distill the two teacher models into one student model
    - Stage 2: Progressive Dstillation - distill the learned model from the first-stage into a fewer-step guided model by halving the number of steps each time
- [DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation](https://cvpr.thecvf.com/virtual/2023/poster/21256)
  - Using a small number of input images, you can create a pre trained text-to-image model to generate images of a specific subject
  - This is difficult to do with text prompts or CLIP embeddings
  - Would be a great method for keeping consistent characters across images
  - Should look into how to implement this
- [3D Registration With Maximal Cliques](https://cvpr.thecvf.com/virtual/2023/poster/22705)
- [DynIBaR: Neural Dynamic Image-Based Rendering](https://cvpr.thecvf.com/virtual/2023/poster/22802)
- [Planning-Oriented Autonomous Driving](https://cvpr.thecvf.com/virtual/2023/poster/22922) - Best Paper Winner
  - Great overview of how many vision models are combined to create aan autonomous driving system.
  - Good reference for the latest SOTA models for various tasks 
- [Integral Neural Networks](https://cvpr.thecvf.com/virtual/2023/poster/21686)
  - They introduce a new family of deep neural networks, where instead of the conventional representation of network layers as N-dimensional weight tensors, we use a continuous layer representation along the filter and channel dimensions.
  - Notably they discuss how existing models could be converted to this system instead of being rebuilt
  - Leading candidate for the paper I least understood
- [Towards Accurate Image Coding: Improved Autoregressive Image Generation With Dynamic Vector Quantization](https://cvpr.thecvf.com/virtual/2023/poster/22990)
  - By encoding with fixed-size image regions you end up with insufficiency in important regions with dense information and redundancy in unimportant regions with sparse information
  - They proposal variable-length coding based on information density

## Related Work
- [Faith and Fate: Limits of Transformers on Compositionality](https://arxiv.org/abs/2305.18654)
  - Referenced in the "AI Odyssey" keynote
- [Why AI is incredibly smart and shockingly stupid](https://www.ted.com/talks/yejin_choi_why_ai_is_incredibly_smart_and_shockingly_stupid/c?language=en)
  - High-level TED talk similar to her keynote 
- [Mask2Former](https://github.com/facebookresearch/Mask2Former)
  - Top image segmentation result from Facebook
