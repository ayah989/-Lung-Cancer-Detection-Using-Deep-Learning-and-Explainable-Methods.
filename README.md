# -Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods.
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/32d39b0b-e98a-490a-b528-24d47389db29)
InceptionV3 confusion matrix    
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/b332a7ac-0cc7-4bd2-aaa6-a4cef3a16b5d)
ResNet50 confusion matrix
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/3f58d81f-06ce-4c11-b8ad-4e1b388eaec1)
ResNet explainable by LIME for cancer
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/9adaa99e-5fe1-494e-b258-63daf5c08385)
InceptionV3 explainable by Grad-Cam for cancer
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/1c466219-6a1f-422e-a8c1-1fd1d2a4169c)
The difference between a radiologist and a LIME diagnosis
Grad-CAM is used to highlight regions of the image that the model used to make it is a prediction of whether or not a patient has lung cancer but the model is making a wrong prediction, Grad-CAM has highlighted regions of the image that are likely irrelevant or not indicative of lung cancer, which leads to a false understanding of the model's decision-making process as ‘Fig.9’ shown the radiologists determine the cancer cells on the original images while the Grad-CAM focuses on the opposite site, and they think the model failed to classify the images because of the very small size of cancer cells and the model need to train on more images like this to develop the performance.
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/c121b438-5ffa-4c46-ace1-29e99f0e9e94)
InceptionV3 results show that in four misclassified images, the model predicts it is a normal image while the actual value it is lung cancer CT images, so the radiologists defined the most important features by the square mark.
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/d2f8dc37-f08c-45e9-82f4-edee3e53ea2a)
According to the figure above the explainable model LIME focuses on different irrelevant features inside and outside the lung, the cancer cells are already covered by LIME highlight but the problem is that focuses on another feature.
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/307d05b1-2e55-4343-8cd1-11f087fde79c)
 the Grad-CAM also failed to explain lung cancer and it highlighted an empty area from the images. 
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/a39b0ec8-26dc-4bfa-80be-83fe2b267f2f)
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/6c106010-c706-41e2-b39a-15103fb8ac0e)
Due to the use of data augmentation in the two figures above considered as a derived image from ‘Fig.10’ and ‘Fig.11’, InceptionV3 failed to classify the original and augmented images maybe because of the low resolution of the images. 
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/9adb9cac-0b5d-4e71-be9c-55148befaa6e)
![image](https://github.com/ayah989/-Lung-Cancer-Detection-Using-Deep-Learning-and-Explainable-Methods./assets/112970757/2d4d01cd-bbff-418f-97af-9d819f2f69f4)
In the figures above InceptionV3 failed to classify the images as lung cancer. According to the explanation by LIME and Grad-CAM, the models highlighted many areas that do not relate to cancer cells in addition to highlighting cancer cells. on the other hand, the radiologists mark the cancer by the yellow square and they think the model fails to classify the images because the big size of cancer cells is not common and the model needs to train on more images like this to develop the performance.

 *****
 The models ResNet50 and InceptionV3 gave a high accuracy in classifying lung cancer images but were found to focus on the wrong features in some images, it is means that the model is not properly identifying the characteristics of cancer. This leads to false positives or false negatives, which can have serious consequences in a clinical setting.
In this scenario, it is important to re-evaluate the model's performance and identify the reasons why it is focused on the wrong features. Additionally, radiologists play a crucial role in identifying the problem and providing feedback on the model's performance and which features are most important for accurate diagnosis. Addressing the problem of focusing on the wrong features, such as the bad image resolution can be a contributing factor to a deep learning model focusing on the wrong features when classifying lung cancer images. When an image has low resolution, it can be more difficult for the model to distinguish important features such as tumors or nodules, which can lead to the model focusing on other, less relevant features instead. also, low-resolution images can result in a loss of important details and textures, which can further complicate the model's ability to accurately identify and classify cancerous regions.



