### **Detection Of Malaria Using Transfer Learning with SVM**  

Transfer learning is popular in the fields of image processing and NLP(Natural language Processing). It is a research problem in machine learning which deals with the usage of a pre-trained model on a huge dataset and using it to train on a similiar and smaller dataset. In general, to train a deep learning model with good accuracy would take 10-20 epochs. With transfer learning a model with great accuracy can be built with just **2-5** epochs. The computational cost is low due to the usage of pre-trained weights.  

Here, different deep learning models were built using transfer learning with SVM and their performance is analyzed.

Different transfer learning models used include Inception_V3, VGG19 and Mobilenet_V2.  
The transfer learning model is used for **feature extraction** and a fully connected layer is built using **SVM** as classifier.

A 70-train, 15- validation and 15- test data split is used. For feature extraction, the transfer learning model is freezed with pretrained weights by excluding the top fully connected layer. A fully connected layer is built using SVM classifier with kernel regularizer = 0.001. The layer is then added to the pretrained model. The model is trained for **5 epochs**. It is observed that the model accuracies obtained with Inception_V3,VGG19 and mobilenet_V2 is 94.4, 86.8 and 89.8.

Inception_V3 with SVM classifier provided the best accuracy of all models built.

Dataset was downloaded from "https://www.kaggle.com/iarunava/cell-images-for-detecting-malaria"
