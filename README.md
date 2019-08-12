#  Project Background  
##  Image-based & Object-based Deep Learning for Vehicle Interiors 

Modern Dashboards can accommodate a broad array of gauges, climate controls, infotainment, and entertainment systems, which contrast to the earlier simpler controls of only speed, fuel, and oil pressure. Automakers have different and distinct ways of designing their dashboards and using a collection of visual identification tools, machine learning and deep learning algorithms we will learn to leverage vehicle features of the dashboard to identify the vehicle and its characteristics. 

The goal of this project is to develop a machine learning model that can help identify the content of a vehicle and its features using visual cues from its interior images of the vehicle. This is a multiclass supervised classification problem that will require labeled images to learn the features from curves, edges, and combination of features.  Our dataset consist of images collected from the CompCar dataset.


##  Deep Learning Models

### Tasks
1.  Image Classification
2.  Object Detection
3.  Demo

Tensorflow 2.0, Tensorflow JS and Tensorflow Hub were used.  

1.  Image Classification done using a pre-trained model as the base and different classifiers, feature extractors, and fine tuning on a custom dataset. 
        classifier_url = 
        feature_extractor_url =
   
2.  Object Detection
    Faster RCNN Inception V2 coco   
    Single-Shot Multibox Detector (SSD) with feature extraction head from MobileNet   
    SSD Lite Mobilenet V2
    SSD Mobilenet V2


 
## Summary of Benchmarks  

| Framework    | N | # Layers | MinTestError | s / epoch |
|--------------|--:|---------:|-------------:|----------:|
| Keras(TF)    | 3 | 20       | 0.0965       | 51.817    |
| Keras(MXNet) | 3 | 20       | 0.0963       | 50.207    |
| Chainer      | 3 | 20       | 0.0995       | 35.360    |
| PyTorch      | 3 | 20       | 0.0986       | 26.602    |  




|Make (Top 1)   | Interior  |  steering |  odometer |   control |   gear    |   All     |
                                wheel                   center      lever
|:-------------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|
|MobileNet      |   0.946   |   0.885   |   0.804   |   0.906   |   0.857   |   0.844   |
|SSD            |   0.953   |   0.949   |   0.259   |   0.777   |   0.789   |   0.767   |
|Overfeat       |   0.710   |   0.521   |   0.507   |   0.680   |   0.656   |   0.829   |


|Faster_rcnn_inception_v2_coco    
|Ssd_inception_v2_coco        
Single-Shot Multibox Detector (SSD) with feature extraction head from MobileNet


##  Product Demo    
![Demo](https://github.com/StephanieRogers-ML/deep-learning_vehicle-dashboard/blob/master/Sample_Data/uploadbox.png)




##  Contact us  

Stephanie Rogers | gp5880@wayne.edu  | stephanierogers.ml@gmail.com  

Jatin Gongiwala  | jatinmg97@wayne.edu |  Jatinmg97@gmail.com  

Ranjitha Vidyashankar  | gm8135@wayne.edu | ranjithavshankar@gmail.com  



