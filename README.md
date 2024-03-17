**Image Domain Transfer using CycleGAN**

This project implements a CycleGAN model for image domain transfer. CycleGAN is a type of generative adversarial network (GAN) that can be used to learn mapping between two different image domains without requiring paired data.

**Project Structure:**

- build_blocks.py: Contains functions to build basic blocks used in the CycleGAN model, such as the reflection padding layer, residual block, and downsampling/upsampling blocks.
- models.py: Defines the generator and discriminator models for the CycleGAN.
- train.py: Defines the training loop for the CycleGAN model.
- utils.py: Contains utility functions for data preprocessing and visualization.

**Usage:**

- Data Preparation: Prepare your dataset with images from the two domains you want to transfer between (e.g., apples to oranges).
- Model Creation: Use the functions in build_blocks.py to create the generator and discriminator models.
- Training: Use the train.py script to train the CycleGAN model on your dataset. You can specify hyperparameters such as the learning rate and batch size in the script.
- Inference: After training, you can use the trained generator to perform domain transfer on new images. Use the transform_image function in utils.py to apply the transformation to a single image.
- Results: Visualize the results of the domain transfer using the plot_results function in utils.py.

**Results:**
After training the CycleGAN model, you should see images from one domain transformed to resemble images from the other domain. The model should be able to learn meaningful mappings between the two domains, even without paired training data.

**Dependencies**
This project requires the following Python libraries:

- TensorFlow 2.x
- Matplotlib
- NumPy
- PIL

**Credits**
This project is inspired by the original CycleGAN paper by Jun-Yan Zhu et al. (2017) and the TensorFlow implementation by Erik Linder-Norén.
