# Train a `CNN` with `data augmentation` - Example using `Flowers102` dataset

In this video, I tried to show how data augmentation can be implemented to train a __Convolutional Neural Network (CNN)__ using the deep learning framework __PyTorch__. I used `Flowers102` dataset for this task, which contains 102 different types of flowers. Data augmentation is a technique which is used to increase the diversity of the training dataset in order to ensure better generalization in the case of unseen (__test__) dataset. It helps reduce overfitting (you can notice the sudden increase in the _test loss_ for the model trained without data augmentation).

From the following two pictures, you will see that the gap between train and test loss & accuracy reduced considerably after using data augmentation.

- ## Without augmentation:

![loss_&_accuracy_without_augmentation.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2058/loss_&_accuracy_without_augmentation.png "loss_&_accuracy_without_augmentation.png")

- ## With augmentation

![loss_&_accuracy_with_augmentation.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2058/loss_&_accuracy_with_augmentation.png "loss_&_accuracy_with_augmentation.png")

Two `.ipynb` files are available in the repository:
- `flowers102_wda.ipynb`: It cantains the code without data augmentation.
- `flowers102_da.ipynb`: It contains the code with data augmentation.

The text file `flowers102_label_names.txt` has the class names of 102 flowers.
