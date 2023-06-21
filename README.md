# CVPR_2023
Notes and work related to the conference

## Keynotes and Panels

- [Revisiting Old Ideas With Modern Hardware](https://cvpr.thecvf.com/virtual/2023/eventlistwithbios/2023KeynotesPanels)
  - Great talk highlighting some of the history of CV and how old ideas returned as technology improved
  - Highlighted challenges with predicting where AI will go in the future
- History and Future of Artificial Intelligence and Computer Vision
- An AI Odyssey: the Dark Matter of Intelligence
- Vision, Language, and Creativity
- Modeling Atoms to Address Our Climate Crisis
- Scientific Discovery and the Environment  

## Tutorials and Workshops
- [Vision Transformer: More is Different](https://cvpr.thecvf.com/virtual/2023/tutorial/18572)
- [Recent Advances in Vision Foundation Models](https://cvpr.thecvf.com/virtual/2023/tutorial/18558)
- [Full-Stack, GPU-based Acceleration of Deep Learning](https://cvpr.thecvf.com/virtual/2023/tutorial/18561)
- [Large-Scale Visual Localization](https://cvpr.thecvf.com/virtual/2023/tutorial/18551)

## Papers

- [Visual Programming: Compositional Visual Reasoning Without Training](https://cvpr.thecvf.com/virtual/2023/poster/22652)
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
