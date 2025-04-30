# 🎓 from gans to clip: a hands-on journey in generative ai with pytorch

i'm currently learning to implement generative ai architectures from scratch using pytorch. this repository documents my hands-on learning journey—from basic gans to more advanced models and multimodal ai systems. it includes detailed implementations, experiments, and key insights along the way.

---

## ✅ completed modules

### 🧱 coding a basic generative architecture
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

---

### 🚀 coding an advanced generative architecture (wgan-gp with celeba)

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
   - 
---

## 🔜 Upcoming Modules

- **combining gans + clip**  
  Generating images from text using hybrid generative architectures.

- **clothing editing with segmentation + generation**  
  Modifying clothing items in images with segmentation and generative AI.

- **visual experimentation with multimodal models**  
  playing with text-image interaction using transformer-based models like CLIP.

- **and more, hopefully!**
