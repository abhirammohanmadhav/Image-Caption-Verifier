# Image-Caption-Verifier:
The image caption verifier works in three sifferent stages:
1) A caption generator model is run. 
2) The generated caption is fed to a Text2Image converter.
3) The generated and the reference images are compared on the basis of how similar they are, to each other. 

# Different similarity metrics:
For this image caption verifier, amongst the various similarity methods, Structural Similarity Index (SSIM) and Mean Square Error (MSE) are computed.
The SSIM takes into account the brightness, contrast, and structure of the two images to compute a similarity score. The value ranges between -1 and 1, where a value of 1 indicates a perfect match. On the other hand MSE calculates the mean of the squared difference between each pixel in the two images. The lower the MSE value, the more similar the images are. The other methods include Normalised Cross COrrelation (NCC), Histogram comparison, etc. For this particular case, SSIM would be a better choice as both the images contain dog and the man and SSIM considers structural similarity of the images.

To improve the image generation capability from text, I have a few suggestions:
1) Increase the size of the image dataset: One way to improve the quality of image descriptions is to increase the size and diversity of the image dataset used for training the model. This can help the model learn fine features and patterns in images, which can lead to more accurate and detailed descriptions.

2) Incorporate more context: Contextual information, such as the location, time, and geographical setting of an image, can provide important cues for generating accurate image descriptions. By incorporating this additional information into the model's training data or input, the model may be able to generate more accurate and relevant descriptions.

3) Fine-tune the model: Fine-tuning involves training the model on a smaller dataset that is similar to the task at hand. By fine-tuning the model on a dataset specifically designed for generating image descriptions, the model can learn to generate more accurate and relevant descriptions.

