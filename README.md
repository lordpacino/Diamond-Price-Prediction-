# Diamond Price Prediction 

## 1. Summary
The purpose of this project is to predict the price of a diamond based on the following features:
- 4C (cut, clarity, color, carat)
- dimensions (x, y, z)
- depth
- table
The dataset for this project is obtained from https://www.kaggle.com/datasets/shivam2503/diamonds 

## 2. IDE and Framework
This project uses Spyder as the IDE. The main framework used in this project are Pandas, Numpy, Scikit-learn and TensorFlow Keras.

## 3. Methodology

### 3.1 Data Pipeline
The data are preprocessed using scikit-learn ordinal encoder on the categorical features and the unwanted column of the data are removed.

### 3.2 Model Pipeline
A feedforward neural network is constructed that is catered specifically for regression problem. The structure of the model is shown as in figure below.

![pipeline baru](https://user-images.githubusercontent.com/76200485/165477693-be0684ee-9ac4-4ed4-839d-f97fdf5a9f4b.png)


The model is trained with a batch size of 64 and for 100 epochs. Early stopping is applied in this training to prevent overfitting. The training stops at epoch 20, with a training MAE of 645 and validation MAE of 379. 

## 4. Results
Prediction are made on the test data. The evaluation of the test data prediction are shown in the figure below.

![baru](https://user-images.githubusercontent.com/76200485/165477805-66834afc-c083-4dce-be6a-9360d972bbd1.jpg)


Figure below shows the graph of predictions versus labels of the test data. 

![result](https://user-images.githubusercontent.com/76200485/165477910-020dbffb-bb6a-47e4-a55a-546edb18b62a.png)
