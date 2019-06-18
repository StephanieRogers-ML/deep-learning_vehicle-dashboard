#  Project Background  

Modern Dashboards can accommodate a broad array of gauges, climate controls, infotainment, and entertainment systems, which contrast to the earlier simpler controls of only speed, fuel, and oil pressure. Automakers have different and distinct ways of designing their dashboards and using a collection of visual identification tools, machine learning and deep learning algorithms we will learn to leverage vehicle features of the dashboard to identify the vehicle and its characteristics. 

The goal of this project is to develop a machine learning model that can help identify the content of a vehicle and its features using visual cues from its interior images of the vehicle. This is a multiclass supervised classification problem that will require labeled images to learn the features from curves, edges, and combination of features.  


##  Vehicle Interior Image Dataset

Our dataset consist of images collected from CompCar.


##  Deep Learning Model

* Image Classification
  Pre-trained GoogLE Net trained on Imagenet & finetuned on exterior CompCar (caffe-multigpu, prototxt files)  
  EfficientNet   
* Object Detection
  Faster RCNN 
* A^3M Architecture  

Requirements: software  
    Requirements for Caffe and pycaffe (see: Caffe installation instructions)  
    Note: Caffe must be built with support for Python layers!  

```make
# In your Makefile.config, make sure to have this line uncommented
WITH_PYTHON_LAYER := 1
```
    Caffe build with mkl, cudnn is strongly recommended. 2. For fast-rcnn based classification experiments, fast-rcnn is needed. 3. For     xgboost based experiments, xgboost is needed. 4. Python packages you might not have: python-numpy, python-scipy, python-matplotlib,     python-opencv, python-scikit-learn.

Requirements: hardware  
For training large CNN networks (VGG16, GoogleNet), a good GPU (e.g., Titan, K20, K40, ...) is needed.  
Other non-deep-learning methods have no specific hardware requirements.    



##  Evaluation  

##  Product Demo    
1.  Upload Photo
![Alt text]
(https://github.com/StephanieRogers-ML/deep-learning_vehicle-dashboard/Sample_Data/uploadbox.png)


##  Contact us  

Stephanie Rogers | gp5880@wayne.edu  | stephanierogers.ml@gmail.com


