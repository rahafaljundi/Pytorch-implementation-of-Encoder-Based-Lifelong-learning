# Pytorch-implementation-of-Encoder-Based-Lifelong-learning

The code contains a demo demonstrating running EBLL on a sequence of two tasks:
1- You need first to have alexNet model trained on one dataset (Task 1) say scenes.
2- The autoencoder should be trained on the data from the first task using that first task data.
3- Given the second task (say CUB) and assuming that the first task data is not available any more, a warmup phase is performed to train the head of the second task, following LwF stratigy.
4- The shared model is trained on the second task using second task data and based on the autoencoders to reduce forgetting.

Note that you need to replace the pathes with your own and add your own datasets. Note that the code assumes an AlexNet based model.


