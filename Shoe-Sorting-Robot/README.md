This is a group project that has design a robot which is able to detect shoes, pair shoes, plan its path to the shoe rack and 
plan its manipulator trajectory in the task space. Although I was only responsible for detecting and pairing task, it was my very first AI related project and
I manage to successfully train my own YOLO in detecting different shoe type as well as the gripping point from scratch. I know it wasn't a difficult task but for a 
completely "newbie" who has spent month setting up the envrionment, annotation by hand, configure all the training files all by myself and even purchase a Colab Pro
for a faster training time, I still feel quite accomplished :)

Colab Notebook link for training YOLO: https://drive.google.com/file/d/1n-a0a56Ml6FJTYG-RLqr-tNLUdF19wZi/view?usp=sharing

https://user-images.githubusercontent.com/110743264/190171354-3364213f-9504-4b66-95b8-49deabe31e03.mp4

For the paring task, I use the Scale Invariant Feature Transform or the SIFT algorithm. As shown below, the result is quite good.

![image](https://user-images.githubusercontent.com/110743264/190172651-a5782f3f-c1b9-44e5-bbfc-31d729087fa3.png)

For other parts of the project, other members were in charge of implmenting SLAM to buildup the environment, path planning the robot to go to the destination,
and path planning the manipulator to grip the shoe.
