This presonal project use RNN to classify text messages is spam or not.

Colab Notebook link: https://colab.research.google.com/drive/1Mw3CK3kKQ7bvziYPs_4yZNYIkesQMyZc?usp=sharing

I use the LSTM instead of the tradition RNN to deal with the vanishing gradient problem. The best model has the following performance:

![image](https://user-images.githubusercontent.com/110743264/190037746-dea7fd57-0f67-43e5-b9d4-04b4517c50a1.png)

The model can classify a message correctly in a reasonable error:

![image](https://user-images.githubusercontent.com/110743264/190039345-cfd93e39-b8ca-4ae6-bd46-109950192a54.png)

Next part I use the Universal Language Model Fine-tuning or the ULMFiT method based on fastai library to perform a transfer learning. Following is the
confusion matrix of the model and some classification perfrom by the model:

![image](https://user-images.githubusercontent.com/110743264/190163147-a318c429-8b47-4a58-a2eb-e326e9db5906.png)

![image](https://user-images.githubusercontent.com/110743264/190163462-db3de0e4-5408-4d05-82f3-d94fc7bebb51.png)

![image](https://user-images.githubusercontent.com/110743264/190163510-ff97bd72-67b2-4401-94b0-904dbf6f05ac.png)

