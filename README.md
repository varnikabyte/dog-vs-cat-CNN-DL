# Cat vs Dog Classifier

I built this while learning the basics of CNNs — it's a simple deep learning model that looks at a photo and tells you whether it's a cat or a dog.

## About the Project
This was my hands-on intro to Convolutional Neural Networks. Instead of just reading theory, I wanted to actually build one from scratch and see how it performs on real images.

## How the Model Works
The CNN has 3 convolutional blocks that gradually pick up on patterns in the images — starting with simple edges and textures, and building up to more complex shapes. Each block uses:
- Conv2D layers (32 → 64 → 128 filters)
- Batch Normalization (keeps training stable)
- Max Pooling (shrinks the image while keeping important features)

After that, it flattens everything and passes it through a couple of dense layers with Dropout (to avoid overfitting), ending in a single output that predicts cat or dog.

## Tools Used
- Python
- TensorFlow / Keras
- OpenCV
- Matplotlib
- Google Colab (for free GPU access)

## What I Did
1. Loaded and preprocessed the images (resized to 256×256, normalized pixel values)
2. Built the CNN architecture
3. Trained it for 10 epochs, tracking accuracy and loss
4. Plotted the training/validation curves to see how well it learned
5. Tested it on new images to check predictions

## What I Learned
This project helped me actually understand how CNNs "see" images layer by layer, and how things like Batch Normalization and Dropout make a real difference in training. It also gave me practice handling image datasets end-to-end — from raw files to a working prediction.
