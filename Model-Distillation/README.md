<p align="justify"> This is project that aims to distill the knowledge from a teacher model with high structural complexity into a student model with <b>shallower</b> structure and has a <b>similar</b> performance compared with the teacher model. With a <b>simpler structure</b> and a <b>smaller FLOPS</b> (floating point operations per second), the studnet model can be deploy on the device with <b>limited computational power</b> and still has a <b>reasonable performance</b>.


<p align="justify">For MNIST dataset, the teacher model will be a convolutional neural network and student will be a fully connected network. From the table we can see that the student's performance drop is insignificant compared to the decrease in number of parameters and <b>a 10 times drop</b> in FLOPS. </p>

  
|                                | Test Accuracy | Number of Param. | FLOPs    |
|--------------------------------|---------------|------------------|----------|
| Teacher Model                  | 99.19%        | 1,011,466        | 2.2*10^7 |
| Student Trained from Scratch   | 98.21%        | 623,290          | 2.5*10^6 |
| Student distilled from Teacher | 98.75%        | 623,290          | 2.5*10^6 |

<p align="justify">For MHIST dataset, the evaluation metric will be f1 score and AUC since the dataset is unbalanced. The teacher model will be a ResNet50V2 network and student will be a MobileNetV2 network. Both model last 5 layers will be unfreezed to be fine tuned. From the table we can see that same as MNIST dataset, the student's performance drop is relatively minor compared to the decrease in number of parameters and <b>a 10 times drop</b> in FLOPS. </p>


|                                | f1 Score | AUC Score | Number of Param. | FLOPs    |
|--------------------------------|----------|-----------|------------------|----------|
| Teacher Model                  | 0.75     | 0.80      | 3,852,966        | 7.0*10^9 |
| Student Trained from Scratch   | 0.69     | 0.76      | 2,562            | 6.1*10^8 |
| Student distilled from Teacher | 0.72     | 0.78      | 2,562            | 6.1*10^8 |

In both dataset, the result demonstrate the success in distilling the knowledge from a teacher model into a student model. The performance has a slight drop but the structure complexity is redeuced to a great extent.
