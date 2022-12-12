# VolcanoClassification


This is a Volcano Detection and Classification challenge.
First part consists classifying volcano and no volcano images.
Second part is to classify the type of detected volcano.

My work pipeline is shown below:
- Get and understand data
- Preprocess data
- Try fundamental ML models
- Augment data
- Try CNN
- Try Transfer Learning
- Evaluate results

The dataset looks like
- Train Images
- Train Labels
- Test images
- Test labels

The labels of data are
- Volcano? ➡️ 0 No Volcano 1 Volcano Exists
- Type ➡️ 1 - definitely a volcano, 2 - probably, 3 - possibly, 4 - only a pit is visible
- Radius ➡️ The radius of the volcano in the center of the image, in pixels
- Number of Volcanoes ➡️ 0 to 5


Final thoughts
The classes had imbalance and I approached it in 2 ways: 
- 1 Keep the data as a fixed component and try better models as well as more suitable evaluation metrics for imbalance
- 2 Keep models as fixed component and try Upsampling underrepresented classes, follow up with cross validation, generate new images with image processing techniques like add noise, change brightness, rotate etc.


Improvement TO DO's
- Could try other classification transfer learning models Inception, Resnet50
- Didn't tried downsampling the dominant class images
- Try Keras Tuner to tune CNN's more effectively
