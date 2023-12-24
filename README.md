# Ensembles-Model-Training

## Author

Paul Ashioya

## Description

For my project, I leveraged SciKit Learn to conduct a comprehensive analysis of various classifiers, including a random forest classifier, a neural net, and an SVM classifier. The training set served as the foundation for individual classifier training, with performance meticulously recorded on the test set. To mitigate overfitting, I strategically employed a validation set and selected a robust metric for precise performance comparisons.

Taking the exploration further, I experimented with combining these classifiers into a voting ensemble, exploring both soft and hard voting mechanisms. The goal was to create an ensemble that surpasses the performance of each standalone classifier on the training set. Once a successful ensemble was identified, its performance was rigorously tested on the test set, with detailed findings and explanations documented.

In the subsequent phase, I utilized the predictions from the individual classifiers on the validation set to construct a new training set. Each training instance comprised a vector containing predictions from all classifiers for a given image, with the image's class designated as the target. The creation of a classifier, referred to as the blender, marked a significant milestone. This blender, in conjunction with the classifiers, formed a stacking ensemble.

The evaluation of this stacking ensemble on the test set involved making predictions for each image using all classifiers, followed by feeding these predictions into the blender to generate ensemble predictions. A thorough comparison with the previously trained voting classifier was conducted. Additionally, I explored the implementation of a SciKit Learn StackingClassifier to assess whether it yielded superior performance. The results were scrutinized to identify potential improvements and understand the underlying reasons for any observed enhancements in performance.