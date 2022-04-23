# Deeply-Supervised-Nets (DSN)

We implement [[Gallagher et. al, 2014]](https://arxiv.org/abs/1409.5185), and run experiments to test how well their proposed technique (to add a companion SVM objective function to every layer of a neural network) holds in a context not explored by the authors. Whereas the authors focus on applying the technique to CNNs and computer vision datasets (i.e. MNIST, CIFAR), we explore DSNs performance with Multi-layer Perceptrons (MLP) on categorical data.

## File Structure

**```DSN.ipynb```** contains our implementation of the DSN on a [date fruits dataset](https://www.kaggle.com/datasets/muratkokludataset/date-fruit-datasets), and includes code for data processing, model definition, training, and reporting of results.

*How to run this:* This can be run from Google Colab by clicking the "Open in Colab" button shown in the file. However, please note that at the moment, reproducing the plots shown in the ipynb exactly is unlikely, if not at all possible. The model training seems to be unstable, and produces a different plot for every training run.

**```MLP_softmax.ipynb```** contains our implementation of a traditional MLP on the date fruits dataset.

*How to run this:* This file can be run in Google Colab from the link provided in the file. However, you will need to have the ```Date_Fruit_Datasets.csv``` file uploaded to your Google Drive, and will need to change the ```path2dataset``` variable accordingly. One way of getting the the .csv file is by running the cells under the 'Download Dataset' header in ```DSN.ipynb``` on your local computer (i.e. in Visual Studio Code).
