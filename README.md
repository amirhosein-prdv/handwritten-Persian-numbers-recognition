# handwritten-Persian-numbers-recognition
Implementation of DCNN model for handwritten Persian/Arabic numbers that introduced in Below paper by Saqib Ali et al.
- [A recognition model for handwritten PersianArabic.pdf](https://github.com/amirhosein-prdv/handwritten-Persian-numbers-recognition/files/10253591/A.recognition.model.for.handwritten.PersianArabic.pdf)

## Abstract
Recently, artificial intelligence-based applications are universally acknowledged. Digit recognition, particularly Persian/Arabic handwritten digits, has many applications in today’s commercial contexts for example office automation and document processing. However, researcher are struggling in hand-crafted digit scripts due to the presence of different digit writing patterns, cursive nature and lack of large public databases that make the feature extraction process more complex. Therefore, critical investigation is needed to reduce these challenges. In this study, a modified Deep Convolutional Neural Network (DCNN) architecture using three convolutional layers blocks based on convolution, batch normalization, pooling, fully connected and dropout regularization parameters are employed to hinder overfitting and increase generalization performance is proposed to recognize handwritten digits. Initially, digits taken from the HODA database are pre-processed using various steps including smoothing, black and white images to grayscale intensity images conversion and resizing it to a fixed dimension. Then optimal features extraction and recognition of handwritten images are done by the DCNN algorithm. In deep learning domain, optimization algorithms are considered core solution and their performances highly depends on optimization algorithm selection. In this paper, various optimization algorithms such as stochastic gradient descent (SGD), Adam, Adadelta, Adagrad, Adamax, Momentum, RMSprop and Nag are employed for the optimization of proposed DCNN. Moreover, current research also analyzes the role of different epochs to ameliorate optical character recognition (OCR) performance of Persian/Arabic handwritten digits. At the end, we also worked on finding a suitable composition of learning parameters to establish high performance DCNN architecture that conquer the loopholes of traditional methods. Results reveal that the proposed DCNN model achieves state-of-the-art performance and outperform other studies in the literature.

## Dataset
- Some examples of HODA dataset:

![image](https://user-images.githubusercontent.com/65303145/208292984-bbe3b847-b9a3-4e6a-81d1-2c61d9256369.png  "Some examples of HODA dataset")

## Model
- Proposed DCNN architecture:

![image](https://user-images.githubusercontent.com/65303145/208293330-5e0449e9-584d-4500-a659-091296801ed1.png)


## Conclusion

The proposed model automatically generates a feature using DCNN and output prediction using the Softmax function. The experimental results demonstrate that, the proposed approach attains the recognition accuracy of 99.50% for the HODA test dataset. Moreover, this study also analyzes several optimization algorithms using different numbers of epochs to ameliorate handwritten digit performance. All optimization algorithms perform well, but experimental results show Adams encouraging performance compared with other optimizers because it combines the finest characteristics of the AdaGrad and RMSProp optimization algorithms that can handle sparse gradients on noisy data. Adams bias-correction helps in achieving best performance over other algorithms. Many testing and experiments have been postponed due to a shortage of hardware resources. As the feature size increases, so it also increases the training time and other requirements. For these reasons, only images of 40*40*40 pixels were utilized in all experiments to reduce the amount of features, while the proposed approach need be confirmed using alternative image sizes. Moreover, the proposed system use only one CNN classifier and validated using one dataset, which may be biased towards the proposed system.
