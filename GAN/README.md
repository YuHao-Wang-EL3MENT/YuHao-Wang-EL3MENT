This personal project build a generator as well as a discriminator to perform colorization task based on CIFAR-10 horse dataset.

Colab Notebook link: https://colab.research.google.com/drive/1QSxw7fDUztfXpq0iK6kgPuKC3D0QebH1?usp=sharing

First I take the problem as a tradition Regression task and trained a CNN which has the following performance. The first line is the original grey image,
the second line is the original color image and the third line is the image colorized from the CNN:

![image](https://user-images.githubusercontent.com/110743264/190029854-932666fd-ba13-4a5b-9365-588e3208052a.png)

Adding a skip connection to make a UNet and train again for a better result:

![image](https://user-images.githubusercontent.com/110743264/190031509-5b381a8c-75fc-4a5c-b87c-a00a2f36ea31.png)

After that, I build and train a condition GAN with a generator and a discriminator to perform the colorization task. Due to the lack of tunning the hyperparameters,
the result is not as satisfying as it was in the previous part:

![image](https://user-images.githubusercontent.com/110743264/190033912-162bc4fe-97bc-4490-80e2-75d8693a6207.png)

To test the model, I found some online horse image and fed into the conditional GAN model which has the following result. It was not ideal but at at least 
it is consistent with the training result which has the "pinky color" :)

![image](https://user-images.githubusercontent.com/110743264/190035439-48d1455f-2cfc-4f62-9e97-263afabc294d.png)
