# GDSC ITB 2022/2023 - Final Project
---
**Author's Details**

*   Name : Wilbert Josef Tanumihardja
*   Member ID : 220010003
*   Path : Machine Learning/Data Science

## Acknowledgement
I would like to express my deepest gratitude to GDSC ITB Lead 2022/2023 for giving me a precious opportunity to learn, grow, and connect within this great community. Also, I would like to express a lot of thanks to Core Team Members which have been worked hard to giving their best for the success of GDSC ITB.

## Project Details
In this project, I gonna build a deep learning model for predicting univariate time-series data which in this project I'm using [Daily Min Temperature Dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-min-temperatures.csv) from [jbrownlee's GitHub Repository](https://github.com/jbrownlee/Datasets). The dataset contains two columns. Those are Date (which spans from 1 January 1981 to 31 December 1990) and Temperature on that date.

With limited dataset, I'm using windowing techinque in this project to generate more data. I also splitting data for training and validation using 2500 as split point so the training data will have exactly 2500 records and the validation data will have 1500 records.

For the neural network itself, I'm combining 1-D Convolutional, LSTM, and also fully connected layer. With this architecture, the training process can be much faster and can give quite good accuracy. The metric I use in this project is Mean Absolute Error (MAE) because it is straightforward and much more resilient to outliers.

I compiled this model with Adam as optimizer, which can converge faster and Huber loss function as loss function, which less sensitive to outliers.

Finally, I train this model with 20 epochs which resulted accuracy around 80% with loss less than 0.6%.
