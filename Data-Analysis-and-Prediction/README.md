This personal project use dataset online to train a linear regression model. The model take 40 features that describing the airplane's status and make a prediction on
what command the controller should send to control the plane.

Colab Notebook link: https://colab.research.google.com/drive/1lHGqMasv2d1VCeQlpYU3NCz_ui30IIf8?usp=sharing

The raw data is in a csv file which require pre-processing, standardization, and adding a bias. The "x_train_std_one" is the training data that is ready to be
fed into the model:
![image](https://user-images.githubusercontent.com/110743264/190480870-4b4439db-1b58-49d7-a6b8-fd46a6b3c27a.png)
![image](https://user-images.githubusercontent.com/110743264/190480895-718ca3d6-cf02-4d0d-979e-8cee73ebdd98.png)


First I use the Direct Solution to test out the data. After that, some exploration on full-batch GD, mini-batch GD and Stochastic GD is carried. Finally, the different
effect on different batch size as well as learning rate is compared:

![image](https://user-images.githubusercontent.com/110743264/190483274-2e3fd540-7104-437b-9e8e-465fc9cee8e0.png)

![image](https://user-images.githubusercontent.com/110743264/190482382-c48748db-c042-4084-bad4-26758ffb27fb.png)

![image](https://user-images.githubusercontent.com/110743264/190482525-72334e74-031f-42e6-ad6e-6d3d8222dcef.png)

At last, one of the model that has the best preformance is selected and has a decent result regarding the RMSE:

![image](https://user-images.githubusercontent.com/110743264/190482811-640a5c0a-7310-4ace-84a0-6039631d60dd.png)
