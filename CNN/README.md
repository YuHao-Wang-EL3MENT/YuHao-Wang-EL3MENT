This is a personal project that train a CNN on Colab GPU to perform image classification on American Sign Language.

Colab Notebook link: https://colab.research.google.com/drive/1gFgZf-rlsG_nxy5u3j12nuFPCjr945XL?usp=sharing

Following is a screenshot of class "B" under the training set as well as the test set which contains different image of the gesture. There are 8 more classes which is from "A" to "I" that is used to train the model:

![image](https://user-images.githubusercontent.com/110743264/190014518-54b1ad39-d0fc-4c58-aba4-e6629ffa0c78.png) ![image](https://user-images.githubusercontent.com/110743264/190015412-18b175cf-3616-4350-b103-14acb7bcf8ba.png)


There are also some test images that I took myself for each letter:

![image](https://user-images.githubusercontent.com/110743264/190015288-078957e7-6e6c-4026-90ea-7ae19b65d33a.png)

I also use alexNet to perform the transfer learning and successfully extract the feature maps for some images:

![image](https://user-images.githubusercontent.com/110743264/190017065-9ad28037-0236-429b-9dec-043a5e494802.png)


The final result for the model can achieve a 75.4% accuracy on validation set and 69.7% on the test set. However for the personal test set, since there is only 3 pictues for each letter, the model is able to achieve a 100% perfect score due to luck.
