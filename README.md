🎓 from gans to clip: a hands-on journey in generative ai with pytorch

i'm currently learning to implement generative ai architectures from scratch using pytorch. this repository documents my hands-on learning journey—from basic gans to more advanced models and multimodal ai systems. it includes detailed implementations, experiments, and key insights along the way.

---

## ✅ completed modules

### 🧱 [coding a basic generative architecture](basic_gan.ipynb)
1. **importing libraries & visualisation**  
   set up the environment and created utility functions for visualising generated images.

2. **hyperparameters & dataLoader**  
   defined training parameters and built a data loader to feed image batches into the model.

3. **generator class**  
   constructed the generator network responsible for creating fake images.

4. **discriminator class**  
   built the discriminator to distinguish between real and fake images.

5. **optimiser setup & generator testing**  
   configured optimisers and ran initial tests on generator output.

6. **loss functions**  
   implemented loss functions for both the generator and the discriminator.

7. **training loop (generator & discriminator, stats)**  
   trained the generator and the discriminator using batches of real and generated data, and logged visual performance stats.
   
8. **final training run**  
   executed the full training loop and evaluated results across epochs.
   

   <img src="https://github.com/user-attachments/assets/0c6f3f6d-4290-4fc9-b3bf-a7d9c892fffb" width="250"/><img src="https://github.com/user-attachments/assets/8024ae65-ae0a-4a6d-a69a-d08e88058818" width="250"/>
   
   figures: generated & real images (respectively)
   
---

### 🚀 [coding an advanced generative architecture (wgan-gp with celeba)](advanced_gan.ipynb)

1. **concepts and theory**  
   - challenges in basic gans  
   - wasserstein loss  
   - gradient penalty  

2. **setup and libraries**  
   - installed and configured W&B for logging  
   - set training parameters  

3. **model architecture**  
   - constructed improved generator and critic (discriminator) networks  
   - explored convolutional layers and parameter initialisation  

4. **data pipeline**  
   - loaded the celeba dataset  
   - defined dataset, dataloader, and optimisers  

5. **training components**  
   - implemented gradient penalty  
   - setup checkpoint saving/loading  

6. **training process**  
   - training loops for critic and generator  
   - logged training stats and resolved debugging issues  

7. **execution and evaluation**  
   - reviewed and ran the full training  
   - observed sample outputs after a few epochs

<img src="https://github.com/user-attachments/assets/b87961d8-2f8c-4df7-890d-7e1c2c422aeb" width="200"/><img src="https://github.com/user-attachments/assets/1f883913-3f49-414d-a4e8-9f409ab91d83" width="200"/><img src="https://github.com/user-attachments/assets/7dabbb2c-a4c4-4582-b9e8-c7111263a12c" width="200"/><img src="https://github.com/user-attachments/assets/9e00a9d6-d99b-4e3e-81ee-60d9449cee8a" width="200"/>

figures: fake faces (from epochs 1-5-50)  & real faces - respectively.

---

 ### [📝 combining gans + clip 🎨](clip+vqgan.ipynb)  
  generating images from text using hybrid generative architectures.

  1. **multimodal generation setup**
   - importing libraries and defining helper functions
   - setting up hyperparameters and the CLIP model

   2. **model implementation**
   - initialising the transformer-based image generator
   - encoding text prompts and optimising the latent space
   - creating and displaying image crops
   - training loop, parameter optimisation, and running the training
<img src="https://github.com/user-attachments/assets/3c7814d1-3973-43d3-b462-317432d618b3" width="200"/>
<img src="https://github.com/user-attachments/assets/0d899519-0270-4d43-b888-803b679721e5" width="350"/>

   3. **interpolation and visualisation**
   - interpolating between latent points
   - creating videos from interpolation sequences 🎞️

https://github.com/user-attachments/assets/a43a3234-4808-4926-b22b-1eb94a365cdc

   4. **creative enhancements**
   - generating code variations
   - tweaking generation for new textures (Davinci Sfumato section)


## 🔜 Upcoming Modules

- **clothing editing with segmentation + generation**  
  modifying clothing items in images with segmentation and generative AI.

- **visual experimentation with multimodal models**  
  playing with text-image interaction using transformer-based models like CLIP.

- **and more, hopefully!**
