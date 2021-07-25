### **Detection Of Malaria Using Transfer Learning with SVM**  

Transfer learning is popular in the fields of image processing and NLP(Natural language Processing). It is a research problem in machine learning which deals with the usage of a pre-trained model on a huge dataset and using it to train on a similiar and smaller dataset. In general, to train a deep learning model with good accuracy would take 10-20 epochs. With transfer learning a model with great accuracy can be built with just **2-5** epochs. The computational cost is low due to the usage of pre-trained weights.  

Here, a deep learning model is built using a transfer learning model named **inception_v3.**  

Inception_v3 is used for **feature extraction** and a fully connected layer is built using **SVM** as classifier.

A 70-train, 15- validation and 15- test data split is used. For feature extraction, the inceptionv3 model is freezed with pretrained weights by excluding the top fully connected layer. A fully connected layer is built using SVM classifier and kernel regularizer is set to 0.001. The model accuracy obtained is **94.4**
