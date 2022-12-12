# Volcano Classification


This is a Volcano Detection and Classification challenge.
First part consists classifying volcano and no volcano images.
Second part is to classify the type of detected volcano.

# Working Pipeline
- Get and understand data
- Preprocess data
- Try fundamental ML models
- Augment data
- Try CNN feature extraction
- Try Transfer Learning
- Evaluate results

# Labels
- Volcano? ➡️ 0 No Volcano 1 Volcano Exists
- Type ➡️ 1 - definitely a volcano, 2 - probably, 3 - possibly, 4 - only a pit is visible
- Radius ➡️ The radius of the volcano in the center of the image, in pixels
- Number of Volcanoes ➡️ 0 to 5


# Final thoughts
The classes had imbalance and I approached it in 2 ways: 
- First accept the data as a fixed component and try models that are prune to imbalance in datasets (like tree boosted models or powerful feature extractors) as well as more suitable evaluation metrics for imbalance
- Second keep models as fixed component and try Upsampling underrepresented classes, follow up with cross validation, generate new images with image processing techniques like add noise, change brightness, rotate etc.

Since these images were not HD, DL models worked better, CNN was a right fit to extract features and classify binary.
ML Classifiers like Naive Bayes and SVM were the ones I believed the most since they'd be powerful to overcome imbalance if I followed up with XGBoost. 


# Improvement TO DO's
- Could try other classification transfer learning models Inception, Resnet50
- Train longer
- Didn't tried downsampling the dominant class images
- Try Keras Tuner to tune CNN's more effectively
