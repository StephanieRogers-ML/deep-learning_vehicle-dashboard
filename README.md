#  Project Background  

Modern Dashboards can accommodate a broad array of gauges, climate controls, infotainment, and entertainment systems, which contrast to the earlier simpler controls of only speed, fuel, and oil pressure. Automakers have different and distinct ways of designing their dashboards and using a collection of visual identification tools, machine learning and deep learning algorithms we will learn to leverage vehicle features of the dashboard to identify the vehicle and its characteristics. 

The goal of this project is to develop a machine learning model that can help identify the content of a vehicle and its features using visual cues from its interior images of the vehicle. This is a multiclass supervised classification problem that will require labeled images to learn the features from curves, edges, and combination of features.  

##  Vehicle Interior Image Dataset

Our dataset consist of images collected from CompCar.


##  Deep Learning Model
1.  Image Classification  
    Pre-trained GoogLE Net trained on Imagenet & finetuned on exterior CompCar (caffe-multigpu, prototxt files)    
    EfficientNet       
    
            Requirements: software  
            Requirements for Caffe and pycaffe (see: Caffe installation instructions)  
            Note: Caffe must be built with support for Python layers!  

            Requirements: hardware  
            For training large CNN networks (VGG16, GoogleNet), a good GPU (e.g., Titan, K20, K40, ...) is needed.  
            Other non-deep-learning methods have no specific hardware requirements.     

2.  Object Detection  
    Faster RCNN   
    A^3M Architecture    


 
## Summary  

| Framework    | N | # Layers | MinTestError | s / epoch |
|--------------|--:|---------:|-------------:|----------:|
| Keras(TF)    | 3 | 20       | 0.0965       | 51.817    |
| Keras(MXNet) | 3 | 20       | 0.0963       | 50.207    |
| Chainer      | 3 | 20       | 0.0995       | 35.360    |
| PyTorch      | 3 | 20       | 0.0986       | 26.602    |  


|Make (Top 1)   |   Front   |   Rear    |   Side    |   FS      |   RS      |   All     |
|:-------------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
|GoogleNet      |   0.946   |   0.885   |   0.804   |   0.906   |   0.857   |   0.844   |
|VGG16          |   0.953   |   0.949   |   0.259   |   0.777   |   0.789   |   0.767   |
|Overfeat       |   0.710   |   0.521   |   0.507   |   0.680   |   0.656   |   0.829   |

|Model (Top 1)  |   Front   |   Rear    |   Side    |   FS      |   RS      |   All     |
|:-------------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
|GoogleNet      |   0.814   |   0.841   |   0.840   |   0.881   |   0.871   |   0.914   |
|VGG16          |   0.845   |   0.888   |   0.232   |   0.750   |   0.756   |   0.718   |
|Overfeat       |   0.524   |   0.431   |   0.428   |   0.680   |   0.598   |   0.767   |

|Model (Top 5)  |   Front   |   Rear    |   Side    |   FS      |   RS      |   All     |
|:-------------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
|GoogleNet      |   0.831   |   0.851   |   0.854   |   0.893   |   0.883   |   0.926   |
|VGG16          |   0.868   |   0.899   |   0.235   |   0.766   |   0.760   |   0.746   |
|Overfeat       |   0.748   |   0.647   |   0.602   |   0.769   |   0.777   |   0.917   |

##  Product Demo    
![Alt text](https://github.com/StephanieRogers-ML/deep-learning_vehicle-dashboard/blob/master/Sample_Data/uploadbox.png)


```make
# In your Makefile.config, make sure to have this line uncommented
WITH_PYTHON_LAYER := 1
```
    Caffe build with mkl, cudnn is strongly recommended. 2. For fast-rcnn based classification experiments, fast-rcnn is needed. 3. For     xgboost based experiments, xgboost is needed. 4. Python packages you might not have: python-numpy, python-scipy, python-matplotlib,     python-opencv, python-scikit-learn.

##  Contact us  

Stephanie Rogers | gp5880@wayne.edu  | stephanierogers.ml@gmail.com


