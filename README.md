# birds

![image](https://github.com/tylernguyen11/birds/assets/68497574/97230d60-88bc-4a6d-b1f8-1d56fdbed3c5)


For the CSE 455 final project, I joined the Kaggle bird competition.
![image](https://github.com/tylernguyen11/birds/assets/68497574/c1cd07be-9909-40eb-8246-a3a600cd0681)
Clearly it's not very good, but my model is pretty simple and was only trained for 40 epochs (training took a long time). However, considering the number of classes (555), I don't think 37% accuracy is too shabby!

I used transfer learning with ResNet18. For the (last) fully connected layer, I just added a linear transformation that outputs to the 555 classes. I used Adam as the optimizer with learning rate 0.01, and used cross entropy loss as the loss function. I leveraged PyTorch and PyTorch Lightning to make the transfer learning process more simple. If I had more time, I would train for more epochs and add more layers. My main issue was how long training took; each epoch took around 5 minutes to complete using the entire dataset.

Link to notebook:
https://www.kaggle.com/tylernguyen11/birds2
