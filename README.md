# Driver_Distraction_Evaluation
![Screenshot (211)](https://user-images.githubusercontent.com/38711536/144023958-fff1b3d3-c0f6-40b3-81c3-6183ca0d64be.png)

DL Libraries used: Keras, Tensorflow

Working:
Train test dataset split - 80%-20% (Dataset link: https://www.kaggle.com/c/porto-seguro-safe-driver-prediction/data)
1) Training: A CNN model is first tuned and trained(code reference Training: https://github.com/avsk80/Driver_Distraction_Evaluation/blob/main/train.py & 
CNN Model:https://github.com/avsk80/Driver_Distraction_Evaluation/blob/main/model.py) on train dataset and the neuron weights are stored as .h5 file, which is used while predicting a new image.
2) Testing: The accuracy(used Root Mean Squared Propagation as the optimiser) and loss(cross entropy in this case) are measured to give picture about the correctness of the model. In my case I achieved 93% accuracy(code reference: https://github.com/avsk80/Driver_Distraction_Evaluation/blob/main/test.py).
Note: Observed that the accuracy changes from processor to processor but on average over 90% has been observed.
3) The input image is fed to the trained CNN Model and based on the type of distrcation exhibited by the driver the classification is done(code reference: https://github.com/avsk80/Driver_Distraction_Evaluation/blob/main/predict.py).
