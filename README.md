# fetal_HC

The project is a trial to implement the technique described in "Direct estimation of fetal head circumference from ultrasound images based on regression CNN".

paper link: Zhang, J., Petitjean, C., Lopez, P. & Ainouz, S.. (2020). Direct estimation of fetal head circumference from ultrasound images based on regression CNN. Proceedings of the Third Conference on Medical Imaging with Deep Learning, in PMLR 121:914-922
 
  The paper propose to leverage the ability of convolutional neural networks (CNN) to directly measure the head circumference, without having to resort to handcrafted features or manually labeled segmented images.

Head circumference is a fetal biometric that is used to estimate gestational age and monitor growth of the fetus.

Dataset: the training dataset of HC18.
it is public dataset and you can get it from this link: https://hc18.grand-challenge.org/ 

The project is implemented on kaggle and written using Pytorch platform.

For Regression:
1-  Softmax Layer is replaced with Linear regression Layer.
2- Regression loss functions are used as:
    1- Mean Square Error (MSE)
    2- Mean Absolute Error (MAE)
    3- Huber Loss (HL)

The performance of the model is measured with MAE.