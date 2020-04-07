# Tensorflow 2.0 Beta Implementation

### <u>1. References used: </u>
    - https://medium.com/tensorflow/neural-style-transfer-creating-art-with-deep-learning-using-tf-keras-and-eager-execution-7d541ac31398

### <u>2. Libraries used: </u>
    - Keras
    - Tensorflow (Code Compatible with 2.00 alpha & 1.1x version)
    - Scikit-learn
    - Pandas
    - Numpy
    - Matplotlib
    - Pillow
    - Function tools
  
### <u>3. Basic Approach: </u>
    While most of the theory and principles behind neural style transfer is well documented within the code itself the general points of importance are as follows: 
        1. The VGG19 model trained on ImageNet is used in order to save time on learning image features.
        2. Style & Content Layers are selected from the VGG19 Model and are used in computing Style loss & Content Loss values respectively
        3. The formula for content loss is the Euclidean Distance between the output and content images
        4. The formula for style loss is based upon the comparison of their Gram matrices

### <u>4. Changes from Source Article: </u>
    The major changes from the source include:
        - Additional visualizations
        - Compatibility with tf 2.00alpha
        - Additional Content Layers added in to make the content more prominent
        - Minor changes to helper functions

# **Outputs:**

## <u>Content Image</u>
> ![](japanese_garden.jpg)

## <u>Style Image</u>
> ![](picasso_selfportrait.jpg)

## <u>Output Image</u>
> ![](out.jpeg)
