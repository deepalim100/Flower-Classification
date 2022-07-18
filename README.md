# Flower-Classification : 

#### Objective : 
Perform object classification on given dataset.

Note : [ Due to the larger file size , I am unable to upload the zip file of data here]

Here is the link for downloading data : https://s3.amazonaws.com/content.udacity-data.com/nd089/flower_data.tar.gz

#### Steps for Object-classification:
1. Start with the EDA notebook :
- [EDA Notebook](https://github.com/deepalim100/Flower-Classification/blob/main/EDA.ipynb) : Analyzing the dataset.

2. Pre trained the selected model with a self-supervised learning approach. RotationNet (UNSUPERVISED REPRESENTATION LEARNING BY PREDICTING IMAGE ROTATIONS https://arxiv.org/pdf/1803.07728.pdf

which includes the unsupervised training while creating the pseudo labels with classes as mention below::

* class_0 : 0 degree
* class_1 : 90 degree
* class_2 : 180 degree
* class_3 : 270 degree

- [Unsupervised training Notebook](https://github.com/deepalim100/Flower-Classification/blob/main/Unsupervised_classfication_training.ipynb) : Training notebook 

![](EDA_1.png)
 
3. Using the pre-trained model checkpoints further for the Supervised classification task with 102 flower categories.
- [Supervised training Notebook](https://github.com/deepalim100/Flower-Classification/blob/main/supervised-classfication.ipynb)

4. The final prediction score on the test dataset is near 71.00%.
5. Here are some sample prediction images.

![](pred_1.png)
![](pred_2.png)

The loss and accuracy graph-

 ![](loss.png)
![](accuracy.png)


6. KPI - Confusion matrix for some classes with graph

![](confusion.png)
![](graph.png)

7. Go through the summary report for detailed steps .
-[Summary txt file](https://github.com/deepalim100/Flower-Classification/blob/main/Flower_Classification_documentation.txt)
