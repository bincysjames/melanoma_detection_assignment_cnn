Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

Melanoma Detection Assignment - Steps followed
1. Data Reading/Data Understanding → Defining the path for train and test images
2. Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32 and resize the images to 180*180.
3. Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset
4. Model Building & training : Model 1
Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).Choose an appropriate optimiser and loss function for model training .Train the model for ~20 epochs

5. Use data augmentation strategy to resolve overfitting
6. Model Building & training on the augmented data - Model2 :
Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).Use optimiser and loss function for model training Train the model for ~20 epochs

7. Class distribution: Examine the current class distribution in the training dataset
8. Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.
9. Model Building & training on the rectified class imbalance data - Model3

You can download the dataset :- https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

# Result 
ACCURACY='88%'
VALLIDATION_ACCURACY='74%'

The model is not overfitting and due to augmentation the accuracy has significantly increased
Yes class rebalance helped here, as its important to balance out the data set or at least get it close to balance it in
