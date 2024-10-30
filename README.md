# Tuning CNNs to Detect Diabetic Retinopathy

![diabetic retinopathy](https://ocretina.net/wp-content/uploads/diabetic-retinopathy-chart.jpg)

#### ``Objectives``
1. Implement a CNN to detect diabetic retinopathy (DR) from retina images taken using fundus photography under a variety of imaging conditions
2. Improve generalization performance and reduce overfitting using **image transformation** and **data augmentation** techniques
3. Tune hyperparameters of the CNN model

#### ``Context``
Diabetic retinopathy (DR) is an eye condition that  affects blood vessels in the retina. It can cause vision loss and blindness in people who have diabetes. Screening for DR allows earlier and more effective treatment options for millions of people.

#### ``Data``
The original dataset is hosted by Kaggle as part of a [[code competition]](https://www.kaggle.com/c/aptos2019-blindness-detection/) hosted by the Asia Pacific Tele-Opthalmology Society (APTOS) in 2019.

The dataset consists of retina images [images](https://drive.google.com/drive/folders/1sdfUC64Un1iwuiHEehcbijxB54OhU_nd?usp=sharing)) and [labels](https://drive.google.com/drive/folders/1MOlSJBZg7L1HtG5vHPt77ighRvQaGfDg?usp=sharing). 

Our objective will be to **build** and **train** a **CNN** to predict whether or not to refer a patient for DR treatment using the binarized severity of DR in patients:
- no referral if {No DR, mild}
- referral if {moderate, severe, and proliferate DR}