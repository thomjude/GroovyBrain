# GroovyBrain
Coding project which uses a variational auto-encoder (VAE) to create a video of a brain moving to music.

It achieves this by using a VAE to generate images of brains using audio information as latent features, and stitches these together into a video.

(See the video_example.MP4 for an example)

Steps: 
1) First download the training set of brain images (augmented-alzheimer-mri-dataset-v2) from Kaggle. (https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset-v2)
2) Notebook 01 downsizes the images and converts them to a numpy array.
3) Notebook 02 creates and trains the variational auto-encoder to be able to generate images of brains from a latent space.
4) Notebook 03 imports and preprocesses an MP3 audio file. It then uses the spectral features as latent features to generate images from the trained VAE and generate a video using the original audio and VAE-generated images.
